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
- `Description` - A brief description of a model element
- `LongDescription` - A lengthy description of a model element

#### Localization
- `IsLanguageDependent` - Properties and terms annotated with this term are language-dependent

#### Term Restrictions
- `RequiresType` - This is the type to use for all tagging terms

#### Resource Paths
- `ResourcePath` - Resource path for entity container child, can be relative to xml:base and the request URL
- `DereferenceableIDs` - Entity-ids are URLs that locate the identified entity
- `ConventionalIDs` - Entity-ids follow OData URL conventions

#### Permissions
- `Permissions` - Permissions available for a property. The value of 2 is reserved for future use.

| Permission | Value |
|------------|-------|
|    None    |   0   |
|    Read    |   1   |
|  ReadWrite |   3   |

#### Metadata Extensions
- `Immutable` - A value for this non-key property can be provided on insert and remains unchanged on update
- `Computed` - A value for this property is generated on both insert and update
- `IsURL` - Properties and terms annotated with this term MUST contain a valid URL
- `AcceptableMediaTypes` - Lists the MIME types acceptable for the annotated entity type marked with HasStream="true" or the annotated stream property
- `MediaType`
- `IsMediaType` - Properties and terms annotated with this term MUST contain a valid MIME type
- `OptimisticConcurrency` - Data modification requires the use of Etags. A non-empty collection contains the set of properties that are used to compute the ETag

## Capabilities
The Capabilities vocabulary aims to provide a way for service authors to describe certain capabilities of an OData Service.

#### Conformance Level
#### Request Capabilities
#### Supported Preferences
#### Query Capabilities
#### Data Modification Capabilities

## Measures
Terms describing monetary amounts and measured quantities

- `ISOCurrency` - The currency for this monetary amount as an [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) currency code
- `Scale` - The number of significant decimal places in the scale part (less than or equal to the number declared in the Scale facet)
- `Unit` - The unit of measure for this measured quantity, e.g. cm for centimeters or % for percentages
