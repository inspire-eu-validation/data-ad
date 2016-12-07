# Conformance class: Information accessibility, Addresses (DRAFT)

Conformance class for the requirements related to the accessibility of referenced information, for example, information stored in registries (code lists, coordinate reference systems).

To be able to test this conformance class, the encoding of the data set must be known, i.e. this is a parameterized conformance class. The XPath expressions used in this test suite assume that the GML encoding is used. If used with the GML encoding this conformance class has an indirect dependency to the conformance class "GML application schema for Addresses".

This conformance class is part of the [Abstract Test Suite for the INSPIRE Data Specification on Addresses](http://inspire.ec.europa.eu/id/ats/data-ad/3.1).

## Standardization target type

INSPIRE spatial data set

## Dependencies

### Direct dependencies

A direct dependency is another conformance class whose requirements must be met by the data set, too.

| Specification | Conformance class | Parameters | 
| ------------- | ----------------- | ---------- |
| [TG DS Template](http://inspire.ec.europa.eu/id/ats/data-ad/3.1/ad-ia/README#ref_TG_DS_tmpl) | [Information accessibility](http://inspire.ec.europa.eu/id/ats/data/3.0rc3/information-accessibility) | n/a |

### Indirect dependencies

An indirect dependency is another conformance class whose requirements must be met by a related resource.

| Specification | Conformance class | Related resource | Parameters |
| ------------- | ----------------- | ---------------- | ---------- |
| [TG DS-AD](http://inspire.ec.europa.eu/id/ats/data-ad/3.1/ad-ia/README#ref_TG_DS_AD) | [GML application schema, Addresses - Network](http://inspire.ec.europa.eu/id/ats/data-ad/3.1/ad-gml) | INSPIRE spatial data set encoded in GML, Addresses features | n/a |
 
## Feature types <a name="feature-types"></a>

The instantiable feature types are:

* Address
* AddressAreaName
* AddressComponent
* AdminUnitName
* PostalDescriptor
* ThoroughfareName

*Note*: When "features" or "spatial objects" are mentioned in the test cases, this refers only to instances of feature types of this application schema, not to any types specified in any other application schema.

## External document references

The following abbreviations are used in the test text for referring to external documents:

Abbreviation                     | Document name
-------------------------------- | --------------------------------------------------
TG DS-AD <a name="ref_TG_DS_ad"></a>   | [INSPIRE Data Specification on Addresses – Technical Guidelines version 3.1](http://inspire.ec.europa.eu/documents/Data_Specifications/INSPIRE_DataSpecification_AD_v3.1.pdf)
TG DS Template <a name="ref_TG_DS_tmpl"></a>   | [INSPIRE Data Specification Template version 3.0rc3](http://inspire.jrc.ec.europa.eu/documents/Data_Specifications/INSPIRE_DataSpecification_Template_v3.0rc3.pdf)

## Test Cases

| Identifier                                                        | Status   | Test case in [TG DS-ad](#ref_TG_DS_ad)  |
| ----------------------------------------------------------------- | -------- | ------------ |
| [Code lists](http://inspire.ec.europa.eu/id/ats/data-ad/3.1/ad-ia/code-list)  | ready for review  | A.6.1 |
| [Feature references](http://inspire.ec.europa.eu/id/ats/data-ad/3.1/hy-ad/features)  | ready for review  | A.1.4 |

## XML namespace prefixes <a name="namespaces"></a>

The following prefixes are used to refer to the corresponding XML namespaces in all test descriptions:

Prefix         | Namespace
-------------- | -------------------------------------------------
gml            | http://www.opengis.net/gml/3.1
ad3            | urn:x-inspire:specification:gmlas:Addresses:3.0
ad             | http://inspire.ec.europa.eu/schemas/ad/4.0

The following variables are used to refer to the corresponding Xpath expressions in all test descriptions:

Variable       | Value
-------------- | -------------------------------------------------
$features      |  //schema-element(ad:Address) \| //schema-element(ad:AddressAreaName) \| //schema-element(ad:AddressComponent) \| //schema-element(ad:AdminUnitName) \| //schema-element(ad:PostalDescriptor) \| //schema-element(ad:ThoroughfareName) 
