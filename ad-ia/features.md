# Feature references

**Version**: 1

**Purpose**: Verify that referenced features can be retrieved.

**Prerequisites**

**Test method**

* Verify that any feature reference in an association role is publicly accessible via HTTP, i.e. inspect all relevant properties. If a reference (@xlink:href) has a value that starts with "#", verify that an element with a `gml:id` attribute with the referenced identifier exists in the same document. If the reference starts with "http", verify that a HTTP GET request to the URI retrieves an XML document. Otherwise report [brokenLink](#brokenLink).

This data theme currently has the following association roles:

* Address.[component](#component): AddressComponent
* Address.[parcel](#parcel): CadastralParcel
* Address.[parentAddress](#parentAddress): Address
* Address.[building](#building): Building, AbstractConstruction
* AddressAreaName.[namedPlace](#namedPlace): gn:NamedPlace
* AddressComponent.[situatedWithin](#situatedWithin): AddressComponent
* AdminUnitName.[adminUnit](#adminUnit): au:AdministrativeUnit
* ThoroughfareName.[transportLink](#transportLink): tn:TransportLink
* Address.locator.AddressLocator.[withinScopeOf](#withinScopeOf): AddressComponent
* AddressRepresentation.[addressFeature](#addressFeature): Address

**Reference(s)**: 

* [TG DS Template](http://inspire.ec.europa.eu/id/ats/data-ad/3.1/ad-ia/README#ref_TG_DS_tmpl) IR requirement Article 4 (2)

**Test type**: adtomated

**Notes**

## Messages

Identifier  |  Message text (parameters start with '$')
---------------------------------------------------------- | -------------------------------------------------------------------------
brokenLink <a name="brokenLink"/>  |  XML document '$filename', $featureType '$gmlid': The property '$propertyName' has a value '$value' that cannot be retrieved using HTTP. Every code list value must be made available in an online registry. 

## Contextual XPath references

The namespace prefixes used as described in [README.md](http://inspire.ec.europa.eu/id/ats/data-ad/3.1/ad-ia/README#namespaces).

Abbreviation                         |  XPath expression    | Multiplicity    | Voidable
------------------------------------ | ---------------------|-----------------|------------
component <a name ="component"></a>	| //schema-element(ad:Address)/ad:component/@xlink:href | 1..\* | No
parcel <a name ="parcel"></a>	| //schema-element(ad:Address)/ad:parcel/@xlink:href | 0..\* | Yes
parentAddress <a name ="parentAddress"></a>	| //schema-element(ad:Address)/ad:parentAddress/@xlink:href | 0..1 | Yes
building <a name ="building"></a>	| //schema-element(ad:Address)/ad:building/@xlink:href | 0..\* | Yes
namedPlace <a name ="namedPlace"></a>	| //schema-element(ad:AddressAreaName)/ad:namedPlace/@xlink:href | 0..1 | Yes
situatedWithin <a name ="situatedWithin"></a>	| //schema-element(ad:ThoroughfareName)/ad:situatedWithin/@xlink:href or //schema-element(ad:AddressAreaName)/ad:situatedWithin/@xlink:href or //schema-element(ad:PostalDescriptor)/ad:situatedWithin/@xlink:href or //schema-element(ad:AdminUnitName)/ad:situatedWithin/@xlink:href | 0..\* | Yes
adminUnit <a name ="adminUnit"></a>	| //schema-element(ad:AdminUnitName)/ad:adminUnit/@xlink:href | 1 | Yes
transportLink <a name ="transportLink"></a>	| //schema-element(ad:ThoroughfareName)/ad:transportLink/@xlink:href | 0..\* | Yes
withinScopeOf <a name ="withinScopeOf"></a>	| //schema-element(ad:Address)/ad:locator/ad:AddressLocator/ad:withinScopeOf/@xlink:href | 0..1 | Yes
addressFeature <a name ="addressFeature"></a>	| //schema-element(ad:AddressRepresentation)/ad:addressFeature/@xlink:href | 0..1 | Yes
