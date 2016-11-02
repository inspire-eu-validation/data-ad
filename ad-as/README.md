# Conformance class: Application schema, Addresses Simple (DRAFT)

Conformance class for the requirements associated with the application schema. 

To be able to test this conformance class, the encoding of the data set must be known, i.e. this is a parameterized conformance class. The XPath expressions used in this test suite assume that the GML encoding is used. If used with the GML encoding this conformance class has an indirect dependency to the conformance class "GML application schema for Addresses".

This conformance class is part of the [Abstract Test Suite for the INSPIRE Data Specification on Addresses](http://inspire.ec.europa.eu/id/ats/data-ad/3.2).

## Standardization target type

INSPIRE spatial data set

## Dependencies

### Direct dependencies

none

### Indirect dependencies

An indirect dependency is another conformance class whose requirements must be met by a related resource.

| Specification | Conformance class | Related resource | Parameters |
| ------------- | ----------------- | ---------------- | ---------- |
| [TG DS-AD](http://inspire.ec.europa.eu/id/ats/data-ad/3.2/ad-as/README#ref_TG_DS_AD) | [GML application schema, Addresses](http://inspire.ec.europa.eu/id/ats/data-ad/3.2/ad-gml) | INSPIRE spatial data set encoded in GML, Addresses features | n/a |
 
## Feature types <a name="feature-types"></a>

The instantiable feature types in the application schema are:

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
TG DS-AD <a name="ref_TG_DS_AD"></a>   | [INSPIRE Data Specification on Addresses – Technical Guidelines version 3.2](http://inspire.ec.europa.eu/documents/Data_Specifications/INSPIRE_DataSpecification_AD_v3.2.pdf)
TG DS Template <a name="ref_TG_DS_tmpl"></a>   | [INSPIRE Data Specification Template version 3.0rc3](http://inspire.jrc.ec.europa.eu/documents/Data_Specifications/INSPIRE_DataSpecification_Template_v3.0rc3.pdf)

## Test Cases

| Identifier                                                        | Status   | Test case in [TG DS-AD](#ref_TG_DS_AD)  |
| ----------------------------------------------------------------- | -------- | ------------ |
| [Code list values](http://inspire.ec.europa.eu/id/ats/data-ad/3.2/ad-as/code-list-values)  | Draft  | A.1.3, A.6.1  |
| [Constraints](http://inspire.ec.europa.eu/id/ats/data-ad/3.2/ad-as/constraints)  | Draft  | A.1.6  |
| [Address Position](http://inspire.ec.europa.eu/id/ats/data-ad/3.2/ad-as/address-position)  | Draft  | A.1.8  |
| [Address Multiple Position](http://inspire.ec.europa.eu/id/ats/data-ad/3.2/ad-as/address-multiple-position)  | Draft  | A.1.9  |
| [Scope of unambiguousness](http://inspire.ec.europa.eu/id/ats/data-ad/3.2/ad-as/unambiguousness)  | Draft  | A.1.10  |
| [Parent Address](http://inspire.ec.europa.eu/id/ats/data-ad/3.2/ad-as/parent-address)  | Draft  | A.1.11  |
| [Country and Address Components](http://inspire.ec.europa.eu/id/ats/data-ad/3.2/ad-as/country-address-components)  | Draft  | A.1.12  |

## XML namespace prefixes <a name="namespaces"></a>

The following prefixes are used to refer to the corresponding XML namespaces in all test descriptions:

Prefix         | Namespace
-------------- | -------------------------------------------------
ad3            | urn:x-inspire:specification:gmlas:Addresses:3.0
ad             | http://inspire.ec.europa.eu/schemas/ad/4.0
base           | http://inspire.ec.europa.eu/schemas/base/3.3
gml            | http://www.opengis.net/gml/3.2
wfs            | http://www.opengis.net/wfs/2.0
xsi            | http://www.w3.org/2001/XMLSchema-instance
xlink          | http://www.w3.org/1999/xlink
xml            | http://www.w3.org/XML/1998/namespace
