# Constraints

**Version**: 1

**Purpose**: Verify that the features provided in the dataset adhere to the constraints specified in the INSPIRE application schema.

**Prerequisites**

**Test method**

Verify that the OCL constraints listed below that are specified in the UML model of the application schema are met, i.e. validate features against the constraints. For unmet constraints report [constraintViolation](#constraintViolation). 

For constraints that require retrieving a referenced resource and the resource cannot be retrieved, report [brokenLink](#brokenLink). The test accepts the following two types of content in @xlink:href attributes: Either a "#" followed by a @gml:id in the same document or a HTTP URI.

Automated tests:

* An address shall have an admin unit address component spatial object whose level is 1 (Country); OCL: "inv: self.component -> forAll (a1 | exists(a1.parent.oclIsTypeOf(AdminUnitName) and a1.parent.level=1))". Verify that for each [address](#address), an AdminUnitName is referenced in [component](#component) and that it is of [level](#level) 1.
* An address shall have exactly one default geographic position (default attribute of GeographicPosition must be true); OCL: "inv: self.position -> one(a1 | a1.default = true)". Verify that for each [address](#address) that there is only one [GeographicPosition](#GeographicPosition) with value true for the [default attribute](#default).  
* If no post code exists, a post name is required.; OCL: "inv: self.postCode->isEmpty() implies self.postName->notEmpty()". Verify that if there is no [postCode](#postCode) value, there is a [postName](#postName) value.
* If no post name exists, a post code is required.; OCL: "inv: self.postName->isEmpty() implies self.postCode->notEmpty()". Verify that if there is no [postName](#postName) value, there is a [postCode](#postCode) value.
* If no designator exists, a name is required.; OCL: "inv: self.designator->isEmpty() implies self.name->notEmpty()". Verify that if there is no [designator](#designator) value, there is a [name](#name) value.
* If no name exists, a designator is required.; OCL: "inv: self.name->isEmpty() implies self.designator->notEmpty()". Verify that if there is no [name](#name) value, there is a [designator](#designator) value.

**Reference(s)**: 

* [TG DS Template](http://inspire.ec.europa.eu/id/ats/data-ad/3.2/ad-as/README#ref_TG_DS_tmpl) IR requirement Article 4 (2)
* [TG DS-AD](http://inspire.ec.europa.eu/id/ats/data-ad/3.2/ad-as/README#ref_TG_DS_AD)) 5.4

**Test type**: Automated

## Messages

Identifier  |  Message text (parameters start with '$')
---------------------------------------------------------- | -------------------------------------------------------------------------
constraintViolation <a name="constraintViolation"/>  |  XML document '$filename', $featureType '$gmlid': The constraint '$constraint' is violated.
brokenLink <a name="brokenLink"/>  |  XML document '$filename', $featureType '$gmlid': The property '$propertyName' has a value '$value' that cannot be retrieved using HTTP.

## Contextual XPath references

The namespace prefixes used as described in [README.md](http://inspire.ec.europa.eu/id/ats/data-ps/3.2/ps-p-as/README#namespaces).

Abbreviation                                               |  XPath expression
---------------------------------------------------------- | -------------------------------------------------------------------------
address <a name="address"></a> 	| 	//schema-element(ad:address)
component <a name="component"></a>   | //schema-element(ad:Address)/ad:component
component level <a name="level"></a>  | //schema-element(ad:AdminUnitName)/ad:level
GeographicPosition <a name="GeographicPosition"></a> 	| 	//schema-element(ad:address)/ad:position/ad:GeographicPosition
default attribute <a name="default"></a> 	| 	//schema-element(ad:address)/ad:position/ad:GeographicPosition/ad:default
postCode <a name="postCode"></a> 	| 	//schema-element(ad:PostalDescriptor)/ad:position/ad:PostalDescriptor/ad:postCode
postName <a name="postName"></a> 	| 	//schema-element(ad:PostalDescriptor)/ad:position/ad:PostalDescriptor/ad:postName
designator <a name="designator"></a> 	| 	//schema-element(ad:Address)/ad:locator/ad:AddressLocator/ad:designator
name <a name="name"></a> 	| 	//schema-element(ad:Address)/ad:locator/ad:AddressLocator/ad:name
