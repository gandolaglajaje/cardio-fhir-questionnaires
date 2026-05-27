# FHIR SDC Questionnaires

FHIR R4 Structured Data Capture (SDC) questionnaires for cardiology referral workflows.

Built as part of the SSCP FHIR SDC Training (NTHC NIH UP Manila, May 2026).

## Questionnaires

| Form | File | Description |
|------|------|-------------|
| Cardiology Referral | [`cardiology-referral.json`](./cardiology-referral.json) | Standardized intake form for cardiology referrals with CVD risk screening |

## Features

- **Prepopulation** from `%patient` launch context (ID, name, age)
- **Conditional logic** via `enableWhen` (urgency justification, risk-based guidance)
- **FHIR extraction** to `ServiceRequest` resource with SNOMED CT coding
- **Calculated CVD risk score** using FHIRPath
- Risk-based clinical guidance (low / elevated)

## Tooling

- Rendering & debug: [fhirpath-lab.com](https://fhirpath-lab.com)
- FHIR server: [Aidbox FHIR Server](https://aidbox.fhirlab.net)
- EMR rendering: [Beda EMR](https://beda.fhirlab.net)

## Author

**Glajaje C. Gandola**
