# OData-V4.0-Vocabularies
A cheatsheet for OData Core, Capability, and Measures Vocabularies

## Core
Core terms needed to write vocabularies

#### Documentation
#### Localization
#### Term Restrictions
#### Resource Paths
#### Permissions
#### Metadata Extensions

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
