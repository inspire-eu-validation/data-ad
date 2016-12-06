#Country and Address Components

**Version**: 1

**Purpose**: Verify that an address has an association to the name of the country in which it is located and that it has associations to the additional address components necessary to the unambiguous identification and location of the address instance

**Prerequisites**

**Test method**

* Check that an [address](#address) is associated to the name of the country in which it is located, i.e. there is a [component](#component) of [level](#level) 1.
* Check that an [address](#address) has associations to the additional address [components](#component) necessary for the unambiguous identification and location of the [address](#address). 


  
**Reference(s)**: 

* [TG DS Template](http://inspire.ec.europa.eu/id/ats/data-ad/3.2/ad-as/README#ref_TG_DS_tmpl) IR requirement Section 5.5.2 (3)

**Test type**: Automatic/Manual

**Notes**

* Point one (Check that an [address](#address) is associated to the name of the country in which it is located, i.e. there is a [component](#component) of [level](#level) 1.) is already tested in [constraints.md](http://inspire.ec.europa.eu/id/ats/data-ad/3.2/ad-as/constraints.md), OCL constraint "inv: self.component -> forAll (a1 | exists(a1.parent.oclIsTypeOf(AdminUnitName) and a1.parent.level=1))". 

## Messages

n/a

## Contextual XPath references

The namespace prefixes used as described in [README.md](http://inspire.ec.europa.eu/id/ats/data-ad/3.1/ad-as/README#namespaces).

Abbreviation                                               |  XPath expression
---------------------------------------------------------- | -------------------------------------------------------------------------
address <a name="address"></a>   | //schema-element(ad:Address)
component <a name="component"></a>   | //schema-element(ad:Address)/ad:component
component level <a name="level"></a>  | //schema-element(ad:Address)/ad:component/ad:level
