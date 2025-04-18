## Common Field Types



The following table outlines the common data types for fields used in the standard.

Type | Description | Valid Examples
-----|-------------|---------------
String | Standard UTF-8 string but unrestricted in content. Any valid Unicode character can be used. |
ASCIIString | Standard UTF-8 string but limited to the ASCII character set. | 
Boolean | Standard JSON boolean. | `true`<br/>`false`
Enum | String representing an option from a defined list of values<br/>- All possible values **MUST** be provided<br/>- Values **MUST** be in all caps<br/>- Spaces **MUST** be replaced with underscores (`_`)<br/>- Values **MUST** be limited to the ASCII character set. | `"OPTION1"`<br/>`"ANOTHER_OPTION"`<br/>`"VAL_ABC_123"`
NaturalNumber | A natural number (i.e. a positive integer inclusive of zero). | `0`<br/>`1`<br/>`10000`
PositiveInteger | A positive integer (zero excluded). | `1`<br/>`10000`
NegativeInteger | A negative integer inclusive of zero. | `0`<br/>`-1`<br/>`-10000`
Integer | Any positive or negative integer inclusive of zero. | `1`<br/>`0`<br/>`-1`
Number | An integer or decimal number. Can be positive, negative or zero. | `0.1`<br/>`-100.09`<br/>`10`<br/>`90.09`
Base64 | Base64 encoded string as per **[[RFC4648]](#nref-RFC4648)**. | `Q29uc3VtZXIgRGF0YSBSaWdodA==`
DateTimeString | Combined Date and Time string as per **[[RFC3339]](#nref-RFC3339)** (labelled date-time in the RFC). As specified in **[[RFC3339]](#nref-RFC3339)** times **MUST** be offset relative to UTC. | `"2007-05-01T15:43:00.12345Z"`<br/>`"2012-12-25T15:43:00-08:00"`<br/>`"1997-01-12T15:43:00.121Z"`
DateString | Date string as per **[[RFC3339]](#nref-RFC3339)** (labelled full-date in the RFC). | `"2007-05-01"`<br/>`"2012-12-25"`
TimeString | Time string as per **[[RFC3339]](#nref-RFC3339)** (labelled full-time in the RFC). As specified in **[[RFC3339]](#nref-RFC3339)** times **MUST** be offset relative to UTC. | `"15:43:00.12345Z"`<br/>`"15:43:00-12:00"`
CurrencyString | Standard 3 character currency codes as per ISO-4217. | `"AUD"`<br/>`"USD"`<br/>`"GBP"`
RateString | A string representing a percentage (e.g., an interest rate). For example, a rate of 100% would be represented by the value `"1"` and a rate of -100% by `"-1"`<br/>- At least 1 and up to a total of 16 significant digits before a decimal point<br/>- Up to 16 digits following a decimal point if required<br/>- No formatting, e.g., thousand-separating commas. | `"0"` or `"0.0"` (0%)<br/>`"1"` or `"1.0"` (100%)<br/>`"-1.234567"` (-123.4567%)<br/>`"-0.056"` (-5.6%)<br/>`"0.03456789"` (3.456789%)<br/>`"0.2"` (20%)<br/>`"23.456"` (2345.6%)
AmountString | A string representing a monetary amount in currency units with fractional units after a decimal point (e.g., if working with Australian dollars: "123.45" for one hundred and twenty-three dollars and forty-five cents).<br/>- A positive, zero or negative number<br/>- Negative numbers identified with a hyphen (`-`) prefix<br/>- Currency symbols **MUST NOT** be supplied<br/>- At least 1 and up to a total of 16 significant digits before a decimal point<br/>- Minimum 2 digits following a decimal point (more digits allowable but only if required)<br/>- No additional formatting, e.g., thousand-separating commas<br/>- Assumed to be in AUD unless specified otherwise. | `"0.01"`<br/>`"10.00"`<br/>`"1234567.89"`<br/>`"-1001.23"`<br/>`"1.999"`
MaskedPANString | Masked credit card number. Lower case `x` **MUST** be used to mask numbers and only the last four digits **MUST** be exposed to facilitate identification. This type is expected to be used for display so the format **MUST** be logical for this context. | `"xxxx xxxx xxxx 1234"`
MaskedAccountString | Masked bank account number genericised for a variety of account types. **MUST** be represented as the full account number would normally be represented for display (including formatting) but with all digits except the last four replaced with a lower case `x`. This type is expected to be used for display so the format **MUST** be logical for this context. | `"xxxx xxxx xxxx 1234"`<br/>`"xxx-xxx xxxxx1234"`
URIString | A valid URI. | `"https://www.example.com"`
ExternalRef | The format is defined by an external reference such as ISO standard or an RFC. | Swift bank codes using [ISO 9362](https://www.iso.org/standard/60390.html).
