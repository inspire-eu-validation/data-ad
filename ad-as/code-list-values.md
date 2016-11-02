# Code list values

**Version**: 1

**Purpose**: Verify whether all attributes whose value type is a code list take the values set out therein

**Prerequisites**

**Test method**

When an attribute has a code list as its type, verify that the values comply with the definitions and include the values set out in Annex II of the regulation. To pass this tests that any instance of an attribute

* takes only values explicitly specified in the INSPIRE code list register when the code list‘s extensibility is 'none'.

Otherwise report [disallowedCodeListValue](#disallowedCodeListValue).

In the Addresses application schema, the following properties have to be tested:
* [GeometryMethodValue (v3)](#GeometryMethodValue3). Valid values:
  * 1stOrder
  * 2ndOrder
  * 3rdOrder
  * 4thOrder
  * 5thOrder
  * 6thOrder
* [GeometryMethodValue (v4)](#GeometryMethodValue4). Valid values:
  * http://inspire.ec.europa.eu/codelist/GeometryMethodValue/byAdministrator
  * http://inspire.ec.europa.eu/codelist/GeometryMethodValue/byOtherParty
  * http://inspire.ec.europa.eu/codelist/GeometryMethodValue/fromFeature
* [GeometrySpecificationValue (v3)](#GeometrySpecificationValue3). Valid values:
  * 1stOrder
  * 2ndOrder
  * 3rdOrder
  * 4thOrder
  * 5thOrder
  * 6thOrder
* [GeometrySpecificationValue (v4)](#GeometrySpecificationValue4). Valid values:
  * http://inspire.ec.europa.eu/codelist/GeometrySpecificationValue/addressArea
  * http://inspire.ec.europa.eu/codelist/GeometrySpecificationValue/adminUnit1stOrder
  * http://inspire.ec.europa.eu/codelist/GeometrySpecificationValue/adminUnit2ndOrder
  * http://inspire.ec.europa.eu/codelist/GeometrySpecificationValue/adminUnit3rdOrder
  * http://inspire.ec.europa.eu/codelist/GeometrySpecificationValue/adminUnit4thOrder
  * http://inspire.ec.europa.eu/codelist/GeometrySpecificationValue/adminUnit5thOrder
  * http://inspire.ec.europa.eu/codelist/GeometrySpecificationValue/adminUnit6thOrder
  * http://inspire.ec.europa.eu/codelist/GeometrySpecificationValue/building
  * http://inspire.ec.europa.eu/codelist/GeometrySpecificationValue/entrance
  * http://inspire.ec.europa.eu/codelist/GeometrySpecificationValue/parcel
  * http://inspire.ec.europa.eu/codelist/GeometrySpecificationValue/postalDelivery
  * http://inspire.ec.europa.eu/codelist/GeometrySpecificationValue/postalDescriptor
  * http://inspire.ec.europa.eu/codelist/GeometrySpecificationValue/segment
  * http://inspire.ec.europa.eu/codelist/GeometrySpecificationValue/thoroughfareAccess
  * http://inspire.ec.europa.eu/codelist/GeometrySpecificationValue/utilityService
* [LocatorDesignatorTypeValue (v3)](#LocatorDesignatorTypeValue3). Valid values:
  * 1stOrder
  * 2ndOrder
  * 3rdOrder
  * 4thOrder
  * 5thOrder
  * 6thOrder
* [LocatorDesignatorTypeValue (v4)](#LocatorDesignatorTypeValue4). Valid values:
  * http://inspire.ec.europa.eu/codelist/LocatorDesignatorTypeValue/addressIdentifierGeneral
  * http://inspire.ec.europa.eu/codelist/LocatorDesignatorTypeValue/addressNumber
  * http://inspire.ec.europa.eu/codelist/LocatorDesignatorTypeValue/addressNumber2ndExtension
  * http://inspire.ec.europa.eu/codelist/LocatorDesignatorTypeValue/addressNumberExtension
  * http://inspire.ec.europa.eu/codelist/LocatorDesignatorTypeValue/buildingIdentifier
  * http://inspire.ec.europa.eu/codelist/LocatorDesignatorTypeValue/buildingIdentifierPrefix
  * http://inspire.ec.europa.eu/codelist/LocatorDesignatorTypeValue/cornerAddress1stIdentifier
  * http://inspire.ec.europa.eu/codelist/LocatorDesignatorTypeValue/cornerAddress2ndIdentifier
  * http://inspire.ec.europa.eu/codelist/LocatorDesignatorTypeValue/entranceDoorIdentifier
  * http://inspire.ec.europa.eu/codelist/LocatorDesignatorTypeValue/floorIdentifier
  * http://inspire.ec.europa.eu/codelist/LocatorDesignatorTypeValue/kilometrePoint
  * http://inspire.ec.europa.eu/codelist/LocatorDesignatorTypeValue/postalDeliveryIdentifier
  * http://inspire.ec.europa.eu/codelist/LocatorDesignatorTypeValue/staircaseIdentifier
  * http://inspire.ec.europa.eu/codelist/LocatorDesignatorTypeValue/unitIdentifier
* [LocatorLevelValue (v3)](#LocatorLevelValue3). Valid values:
  * 1stOrder
  * 2ndOrder
  * 3rdOrder
  * 4thOrder
  * 5thOrder
  * 6thOrder
* [LocatorLevelValue (v4)](#LocatorLevelValue4). Valid values:
  * http://inspire.ec.europa.eu/codelist/LocatorLevelValue/accessLevel
  * http://inspire.ec.europa.eu/codelist/LocatorLevelValue/postalDeliveryPoint
  * http://inspire.ec.europa.eu/codelist/LocatorLevelValue/siteLevel
  * http://inspire.ec.europa.eu/codelist/LocatorLevelValue/unitLevel
* [LocatorNameTypeValue (v3)](#LocatorNameTypeValue3). Valid values:
  * 1stOrder
  * 2ndOrder
  * 3rdOrder
  * 4thOrder
  * 5thOrder
  * 6thOrder
* [LocatorNameTypeValue (v4)](#LocatorNameTypeValue4). Valid values:
  * http://inspire.ec.europa.eu/codelist/LocatorNameTypeValue/buildingName
  * http://inspire.ec.europa.eu/codelist/LocatorNameTypeValue/descriptiveLocator
  * http://inspire.ec.europa.eu/codelist/LocatorNameTypeValue/roomName
  * http://inspire.ec.europa.eu/codelist/LocatorNameTypeValue/siteName
* [PartTypeValue (v3)](#PartTypeValue3). Valid values:
  * 1stOrder
  * 2ndOrder
  * 3rdOrder
  * 4thOrder
  * 5thOrder
  * 6thOrder
* [PartTypeValue (v4)](#PartTypeValue4). Valid values:
  * http://inspire.ec.europa.eu/codelist/PartTypeValue/name
  * http://inspire.ec.europa.eu/codelist/PartTypeValue/namePrefix
  * http://inspire.ec.europa.eu/codelist/PartTypeValue/qualifier
  * http://inspire.ec.europa.eu/codelist/PartTypeValue/type
* [StatusValue (v3)](#StatusValue3). Valid values:
  * 1stOrder
  * 2ndOrder
  * 3rdOrder
  * 4thOrder
  * 5thOrder
  * 6thOrder
* [StatusValue (v4)](#StatusValue4). Valid values:
  * http://inspire.ec.europa.eu/codelist/StatusValue/alternative
  * http://inspire.ec.europa.eu/codelist/StatusValue/current
  * http://inspire.ec.europa.eu/codelist/StatusValue/proposed
  * http://inspire.ec.europa.eu/codelist/StatusValue/reserved
  * http://inspire.ec.europa.eu/codelist/StatusValue/retired

The following is not applicable for this application schema as no extensions are allowed. It is still included here as a reminder in case extensions will be allowed in the future:

Inspect the code list valued property elements. If a value is not one of the values listed above, review the code list definition to check that any extensions do not overlap with the code lists that are defined in Annexes II, III and IV of the Implementing Rule and that all extensions conform to the requirements. This is a manual test.
  
**Reference(s)**: 

* [TG DS Template](http://inspire.ec.europa.eu/id/ats/data-ad/3.1/au-as/README#ref_TG_DS_tmpl) IR requirement Article 4 (1)
* [TG DS Template](http://inspire.ec.europa.eu/id/ats/data-ad/3.1/au-as/README#ref_TG_DS_tmpl) IR requirement Article 4 (3)
* [TG DS Template](http://inspire.ec.europa.eu/id/ats/data-ad/3.1/au-as/README#ref_TG_DS_tmpl) IR requirement Article 6 (1)l
* [TG DS Template](http://inspire.ec.europa.eu/id/ats/data-ad/3.1/au-as/README#ref_TG_DS_tmpl) IR requirement Article 6 (2)
* [TG DS Template](http://inspire.ec.europa.eu/id/ats/data-ad/3.1/au-as/README#ref_TG_DS_tmpl) IR requirement Article 6 (3)
* [TG DS Template](http://inspire.ec.europa.eu/id/ats/data-ad/3.1/au-as/README#ref_TG_DS_tmpl) IR requirement Article 6 (4)

**Test type**: Automated

**Notes**

## Messages

Identifier  |  Message text (parameters start with '$')
---------------------------------------------------------- | -------------------------------------------------------------------------
disallowedCodeListValue <a name="disallowedCodeListValue"/>  |  XML document '$filename', $featureType '$gmlid': The property '$propertyName' has a value '$value' that is not one of the allowed values listed at $codelist. 

## Contextual XPath references

The namespace prefixes used as described in [README.md](http://inspire.ec.europa.eu/id/ats/data-au/3.1/au-as/README#namespaces).

Abbreviation                                               |  XPath expression
---------------------------------------------------------- | -------------------------------------------------------------------------
GeometryMethodValue (v3) <a name="GeometryMethodValue3"></a>   | //schema-element(ad3:Address)/ad3:/text()
GeometryMethodValue (v4) <a name="GeometryMethodValue4"></a>   | //schema-element(au:Address)/ad:/@href:xlink
GeometrySpecificationValue (v3) <a name="GeometrySpecificationValue3"></a>   | //schema-element(ad3:Address)/ad3:/text()
GeometrySpecificationValue (v4) <a name="GeometrySpecificationValue4"></a>   | //schema-element(au:Address)/ad:/@href:xlink
LocatorDesignatorTypeValue (v3) <a name="LocatorDesignatorTypeValue3"></a>   | //schema-element(ad3:Address)/ad3:/text()
LocatorDesignatorTypeValue (v4) <a name="LocatorDesignatorTypeValue4"></a>   | //schema-element(au:Address)/ad:/@href:xlink
LocatorLevelValue (v3) <a name="LocatorLevelValue3"></a>   | //schema-element(ad3:Address)/ad3:/text()
LocatorLevelValue (v4) <a name="LocatorLevelValue4"></a>   | //schema-element(au:Address)/ad:/@href:xlink
LocatorNameTypeValue (v3) <a name="LocatorNameTypeValue3"></a>   | //schema-element(ad3:Address)/ad3:/text()
LocatorNameTypeValue (v4) <a name="LocatorNameTypeValue4"></a>   | //schema-element(au:Address)/ad:/@href:xlink
PartTypeValue (v3) <a name="PartTypeValue3"></a>   | //schema-element(ad3:Address)/ad3:/text()
PartTypeValue (v4) <a name="PartTypeValue4"></a>   | //schema-element(au:Address)/ad:/@href:xlink
StatusValue (v3) <a name="StatusValue3"></a>   | //schema-element(ad3:Address)/ad3:/text()
StatusValue (v4) <a name="StatusValue4"></a>   | //schema-element(au:Address)/ad:/@href:xlink
