# Conformance class: GML application schema, Addresses Simple (DRAFT)

Conformance class for the GML encoding of spatial objects specified in the INSPIRE GML application schema 'Addresses Simple'. This conformance class examines the data set against requirements associated with the GML application schema. Both currently approved GML application schema versions (3.0 and 4.0) are tested.

This conformance class is part of the [Abstract Test Suite for the INSPIRE Data Specification on Addresses](http://inspire.ec.europa.eu/id/ats/data-ad/3.1).

## Standardization target type

INSPIRE spatial data set encoded in GML, Protected Site features

## Dependencies

### Direct dependencies

A direct dependency is another conformance class whose requirements must be met by the GML documents, too.

| Specification | Conformance class | Parameters | 
| ------------- | ----------------- | ---------- |
| [TG DS Template](#ref_TG_DS_tmpl) | [INSPIRE GML application schemas](http://inspire.ec.europa.eu/id/ats/data/3.0rc3/schemas) | n/a |

### Indirect dependencies

n/a
 
## External document references

The following abbreviations are used in the test text for referring to external documents:

Abbreviation                     | Document name
-------------------------------- | --------------------------------------------------
TG DS-AD <a name="ref_TG_DS_AD"></a>   | [INSPIRE Data Specification on Addresses – Technical Guidelines version 3.1](http://inspire.ec.europa.eu/documents/Data_Specifications/INSPIRE_DataSpecification_AD_v3.1.pdf)
TG DS Template <a name="ref_TG_DS_tmpl"></a>   | [INSPIRE Data Specification Template version 3.0rc3](http://inspire.jrc.ec.europa.eu/documents/Data_Specifications/INSPIRE_DataSpecification_Template_v3.0rc3.pdf)

## Test Cases

| Identifier                                                        | Status   | Test case in [TG DS-AD](#ref_TG_DS_AD)  |
| ----------------------------------------------------------------- | -------- | ------------ |
| [Basic test](http://inspire.ec.europa.eu/id/ats/data-ad/3.1/ad-gml/basic)  | ready for review  | A.1.1, (A.6.1)  |

## XML namespace prefixes <a name="namespaces"></a>

The following prefixes are used to refer to the corresponding XML namespaces in all test descriptions:

Prefix         | Namespace
-------------- | -------------------------------------------------
ad             | urn:x-inspire:specification:gmlas:Addresses:3.0 or http://inspire.ec.europa.eu/schemas/ad/4.0
