# FHIR SDC Questionnaires

FHIR R4 Structured Data Capture (SDC) questionnaires built during the SSCP FHIR SDC Training (NTHC NIH UP Manila, May 2026).

A small collection of forms covering the core SDC patterns: prepopulation, conditional logic, extraction, and score calculation.

## Questionnaires

| Form | File | Description |
|------|------|-------------|
| Cardiology Referral | [`cardiology-referral.json`](./questionnaires/cardiology-referral.json) | Standardized intake form for cardiology referrals with CVD risk screening and extraction to a ServiceRequest |
| Patient Prepopulation | [`patient-prepopulation.json`](./questionnaires/patient-prepopulation.json) | Patient demographics form fully prepopulated from launch context; uses `itemPopulationContext` for a repeating telecom group |
| Vital Signs Extraction | [`vital-signs-observations.json`](./questionnaires/vital-signs-observations.json) | Vital signs intake with template-based extraction producing a list of Observation resources |
| PHQ-2 Depression Screening | [`phq2-score.json`](./questionnaires/phq2-score.json) | Standard 2-item depression screening with calculated total score and clinical interpretation |

## Demonstration

- **Prepopulation** from `%patient` launch context using `initialExpression`
- **Repeating groups** populated via `itemPopulationContext`
- **Conditional logic** via `enableWhen` (single and multi-condition with `enableBehavior`)
- **Template-based extraction** to `ServiceRequest` and `Observation` resources
- **Calculated expressions** in FHIRPath for clinical scoring
- LOINC and SNOMED CT coding for clinical interoperability

## Tooling

- Rendering & debug: [fhirpath-lab.com](https://fhirpath-lab.com)
- FHIR server: [Aidbox FHIR Server](https://aidbox.fhirlab.net)
- EMR rendering: [Beda EMR](https://beda.fhirlab.net)

## Author

**Glajaje C. Gandola**
