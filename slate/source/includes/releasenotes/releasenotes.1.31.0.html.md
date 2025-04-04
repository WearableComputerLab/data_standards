---
title: Consumer Data Standards - v1.31.0 Release Notes

#language_tabs: # must be one of https://git.io/vQNgJ

toc_footers:
  - <a href='../../index.html'>Consumer Data Standards</a>

search: false
---

# V1.31.0 Release Notes
Release notes for version v1.31.0 of the [CDR Standards](../../index.html).

## Changes Made
### Change Requests

This release addresses the following minor defects raised on [Standards Staging](https://github.com/ConsumerDataStandardsAustralia/standards-staging/issues):

- [Standards Staging #377 - Review FDO table](https://github.com/ConsumerDataStandardsAustralia/standards-staging/issues/377)
- [Standards Staging #394 - Fix typo 'registeration'](https://github.com/ConsumerDataStandardsAustralia/standards-staging/issues/394)
- [Standards Staging #395 - Enhancements to Banking documentation](https://github.com/ConsumerDataStandardsAustralia/standards-staging/issues/395)
- [Standards Staging #396 - Improve clarity of the PerformanceMetricsV3 structure](https://github.com/ConsumerDataStandardsAustralia/standards-staging/issues/396)
- [Standards Staging #400 - Enable generic links to schemas](https://github.com/ConsumerDataStandardsAustralia/standards-staging/issues/400)
- [Standards Staging #402 - Update Consumer Data Right link](https://github.com/ConsumerDataStandardsAustralia/standards-staging/issues/402)

This release addresses the following change requests raised on [Standards Maintenance](https://github.com/ConsumerDataStandardsAustralia/standards-maintenance/issues):

- [Standards Maintenance #415 - Disambiguation of the claims for a response from the introspection endpoint](https://github.com/ConsumerDataStandardsAustralia/standards-maintenance/issues/415)
- [Standards Maintenance #615 - Plan Obligation Milestones for 2025](https://github.com/ConsumerDataStandardsAustralia/standards-maintenance/issues/615)
- [Standards Maintenance #633 - Collection Consents - Authorisation Amendment](https://github.com/ConsumerDataStandardsAustralia/standards-maintenance/issues/633)
- [Standards Maintenance #634 - Potential error in Telco specification](https://github.com/ConsumerDataStandardsAustralia/standards-maintenance/issues/634)
- [Standards Maintenance #640 - Retirement date for Get Generic Plan Detail v2 and Get Energy Account Detail v3](https://github.com/ConsumerDataStandardsAustralia/standards-maintenance/issues/640)
- [Standards Maintenance #643 - Update TLS cipher suite requirements to address DHEat Attacks and Raccoon Attack vulnerabilities](https://github.com/ConsumerDataStandardsAustralia/standards-maintenance/issues/643)


### Decision Proposals
This release addresses the following Decision Proposals published on [Standards](https://github.com/ConsumerDataStandardsAustralia/standards/issues):

- [Decision Proposal #347 - Maintenance Iteration 19](https://github.com/ConsumerDataStandardsAustralia/standards/issues/347)


## General Changes
|Change|Description|Link|
|------|-----------|----|
| Enable generic links to schemas | [**Standards Staging #400**](https://github.com/ConsumerDataStandardsAustralia/standards-staging/issues/400): Added anchors to allow linking to a schema base (without a specific version) from guidance material | Applies to all schemas
| Updated Consumer Data Right link | [**Standards Staging #402**](https://github.com/ConsumerDataStandardsAustralia/standards-staging/issues/402): Updated Consumer Data Right website link | [Introduction](../../#introduction)


## Introduction
|Change|Description|Link|
|------|-----------|----|
| Updated FDO table | [**Standards Staging #377**](https://github.com/ConsumerDataStandardsAustralia/standards-staging/issues/377): Removed Future Dated Obligations prior to 2024. Earlier obligations may be viewed in Archived versions | [Future Dated Obligations](../../#future-dated-obligations)<br>[Archives](../../#archives)
| Updated Obligation Date Schedule | [**Standards Maintenance #615**](https://github.com/ConsumerDataStandardsAustralia/standards-maintenance/issues/615): Added 2025 dates to the Obligation Date Schedule and removed dates prior to 2024 | [Obligation Date Schedule](../../includes/endpoint-version-schedule/#obligation-dates-schedule)
| Energy API retirement date change| [**Standards Maintenance #640**](https://github.com/ConsumerDataStandardsAustralia/standards-maintenance/issues/640): Changed retirement date of  Get Generic Plan Detail v2 and Get Energy Account Detail v3 to March 3rd 2025 | [Future Dated Obligations](../../#future-dated-obligations)


## High Level Standards

None


## API Endpoints
|Change|Description|Link|
|------|-----------|----|
| Enhancements to Banking documentation | [**Standards Staging #395**](https://github.com/ConsumerDataStandardsAustralia/standards-staging/issues/395): In addition to minor styling updates, aligned Banking documentation to enhancements applied in the Candidate Standards | [Banking APIs](../../#banking-apis)<br>[Additional Standards](../../#additional-standards)
| Clarified PerformanceMetricsV3 structure | [**Standards Staging #396**](https://github.com/ConsumerDataStandardsAustralia/standards-staging/issues/396): Clarified PerformanceMetricsV3 structure to ensure previousDays arrays are represented correctly | [PerformanceMetricsV3](../../#cdr-admin-api_schemas_tocSperformancemetricsv3)


## Information Security Profile
|Change|Description|Link|
|------|-----------|----|
| Introspection endpoint clarification | [**Standards Maintenance #415**](https://github.com/ConsumerDataStandardsAustralia/standards-maintenance/issues/415): Clarified that a Token Introspection End Point response must include specific fields only for currently active tokens | [Introspection End Point](../../#introspection-end-point)
| Arrangement amendment clarification | [**Standards Maintenance #633**](https://github.com/ConsumerDataStandardsAustralia/standards-maintenance/issues/633): Updated the "Specifying an existing arrangement" section clarifying the requirements for amending existing arrangements | [Specifying an existing arrangement](../../#specifying-an-existing-arrangement)
| Deprecation of vulnerable ciphers | [**Standards Maintenance #643**](https://github.com/ConsumerDataStandardsAustralia/standards-maintenance/issues/643): Allow data holders to deprecate use of vulnerable TLS ciphers | [Ciphers](../../#ciphers)

## Register Standards

None


## Consumer Experience
|Change|Description|Link|
|------|-----------|----|
| Arrangement amendment clarification | [**Standards Maintenance #633**](https://github.com/ConsumerDataStandardsAustralia/standards-maintenance/issues/633): <ul><li>Updated "Authorisation: Amending consent" CX standard noting it needs to align with security requirements for specifiying an existing arrangement.</li><li> Added "Amendment of Collection Consents and Authorisations" CX standard to clarify CDR Arrangement ID is required for consent and authorisation amendments</li></ul> | [Amending Authorisation Standards](../../#amending-authorisation-standards) </br>[Consent Standards](../../#consumer-experience_consent-standards)

## Non-Functional Requirements

None

## Additional Standards
|Change|Description|Link|
|------|-----------|----|
| Fixed typo | [**Standards Staging #394**](https://github.com/ConsumerDataStandardsAustralia/standards-staging/issues/394): Fixed typo in 'Country of registeration' in the Candidate Standards for the Banking and Non-Bank Lending sector | [Additional Standards](../../#additional-standards)
| Removed duplicate TelcoAccount schema | [**Standards Maintenance #634**](https://github.com/ConsumerDataStandardsAustralia/standards-maintenance/issues/634): Removed duplicate `TelcoAccount` schema in the `TelcoAccountDetailResponseData` schema, in the 'Get Telco Account Detail' endpoint in the Telco Candidate Standards | [Additional Standards](../../#additional-standards)


## Known Issues

None
