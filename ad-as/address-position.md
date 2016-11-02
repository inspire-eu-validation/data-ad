# Address Position

**Version**: 1

**Purpose**: Verify whether, in the data set, the position of the address is represented by the coordinates of the actual location with the best available accuracy. This is the most precise directly captured coordinates or, if none exist, then coordinates derived from one of the address components, with priority given to the component that allows the position to be most accurately determined.

**Prerequisites**

**Test method**

* Verify that the coordinates representing the position of the address were directly captured with the best precision.
* If not, identify which address component the coordinates are derived from. 
* Check whether the identified component is the one allowing the position to be most accurately determined.

  
**Reference(s)**: 

* [TG DS Template](http://inspire.ec.europa.eu/id/ats/data-ad/3.2/ad-as/README#ref_TG_DS_tmpl) IR requirement Section 5.5.1 (1)

**Test type**: Manual

**Notes**

## Messages

n/a

## Contextual XPath references

n/a
