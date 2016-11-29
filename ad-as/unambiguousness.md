# Scope of unambiguousness

**Version**: 1

**Purpose**:  Verify whether the withinScopeOf association role is populated for all locators which are assigned according to rules that seek to ensure unambiguousness within a specific address component

**Prerequisites**

**Test method**

* Check that the [withinScopeOf association role](#withinScopeOf) is populated for all [locators](#locator) which are assigned according to rules that seek to ensure unambiguousness within a specific address [component](#component), that is thoroughfare name, address area name, postal descriptor or administrative unit name.
  
**Reference(s)**: 

* [TG DS Template](http://inspire.ec.europa.eu/id/ats/data-ad/3.2/ad-as/README#ref_TG_DS_tmpl) IR requirement Section 5.5.2 (1)

**Test type**: Manual

**Notes**

## Messages

n/a

## Contextual XPath references

The namespace prefixes used as described in [README.md](http://inspire.ec.europa.eu/id/ats/data-ad/3.1/ad-as/README#namespaces).

Abbreviation                                               |  XPath expression
---------------------------------------------------------- | -------------------------------------------------------------------------
withinScopeOf association role <a name="withinScopeOf"></a>   | //schema-element(ad:Address)/ad:locator/ad:AddressLocator/ad:withinScopeOf
locator <a name="locator"></a>   | //schema-element(ad:Address)/ad:locator
component <a name="component"></a>  | //schema-element(au:Address)/ad:component
