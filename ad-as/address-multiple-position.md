# Address Multiple Position

**Version**: 1

**Purpose**: Verify whether, if an address has more than one position, the specification attribute is populated with a different value for each of these.

**Prerequisites**

**Test method**

* Check whether an [address](#address) has more than one [position](#position); in this case, evaluate the [specification attribute](#specification). The test is passed if it have different values for each position.

  
**Reference(s)**: 

* [TG DS Template](http://inspire.ec.europa.eu/id/ats/data-ad/3.2/ad-as/README#ref_TG_DS_tmpl) IR requirement Section 5.5.1 (2)

**Test type**: Automated

**Notes**

## Messages

n/a

## Contextual XPath references

The namespace prefixes used as described in [README.md](http://inspire.ec.europa.eu/id/ats/data-ad/3.1/ad-as/README#namespaces).

Abbreviation                                               |  XPath expression
---------------------------------------------------------- | -------------------------------------------------------------------------
address <a name="address"></a>   | //schema-element(ad:Address)
position <a name="position"></a>   | //schema-element(ad:Address)/ad:position
specification attribute <a name="specification"></a>  | //schema-element(ad:Address)/ad:position/ad:GeographicPosition/ad:specification/@xlink:href or //schema-element(ad3:Address)/ad3:position/ad3:GeographicPosition/ad3:specification/text()
