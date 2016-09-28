# OData-V4.0-Vocabularies
A cheatsheet for OData Core, Capability, and Measures Vocabularies

### Disclaimer
I take no responsibility for the correctness or currency of this data. The authoritative source can be found [here](http://www.odata.org/vocabularies/).

The contents of this document are derived from works bearing the following copyright

```
OData Version 4.0
OASIS Standard
24 February 2014
Copyright (c) OASIS Open 2014. All Rights Reserved.
Source: http://docs.oasis-open.org/odata/odata/v4.0/os/vocabularies/
```

## Core
Core terms needed to write vocabularies

#### Documentation
- `Description`
- `LongDescription`

#### Localization
- `IsLanguageDependent`

#### Term Restrictions
- `RequiresType`

#### Resource Paths
- `ResourcePath`
- `DereferenceableIDs`
- `ConventionalIDs`

#### Permissions
- `Permissions`

#### Metadata Extensions
- `Immutable`
- `Computed`
- `IsURL`
- `AcceptableMediaTypes`
- `MediaType`
- `IsMediaType`
- `OptimisticConcurrency`

## Capabilities
The Capabilities vocabulary aims to provide a way for service authors to describe certain capabilities of an OData Service.

#### Conformance Level
#### Request Capabilities
#### Supported Preferences
#### Query Capabilities
#### Data Modification Capabilities

## Measures
Terms describing monetary amounts and measured quantities

- `ISOCurrency` - The currency for this monetary amount as an [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) currency code<br />Type: `Edm.String`<br />AppliesTo: `Property`

- `Scale` - The number of significant decimal places in the scale part (less than or equal to the number declared in the Scale facet)<br />**Type:** `Edm.Byte`<br />AppliesTo: `Property`<br />RequiresType: `Edm.Decimal`

- `Unit` - The unit of measure for this measured quantity, e.g. cm for centimeters or % for percentages<br />Type: `Edm.String`<br />AppliesTo: `Property`
