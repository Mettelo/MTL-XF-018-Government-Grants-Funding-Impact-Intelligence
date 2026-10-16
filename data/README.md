# Data Guidance

## Approved Core Dataset

Use the Cabinet Office **Government Grants Register 2024–25 — scheme and award data**.

Official source:
https://www.gov.uk/government/statistics/government-grants-statistics-2024-to-2025

The approved core file is the published ODS register containing scheme and award data.

## What to Put in `data/raw/`

Store the original ODS file unchanged:

```text
data/raw/
└── government-grants-register-2024-2025.ods
```

Do not overwrite the ODS with a cleaned spreadsheet.

Processed CSV/Parquet outputs belong in `data/processed/`.

## Core Scope

Use the **full 2024–25 register** for the core project.

Do not arbitrarily restrict the data to a few departments before completing the initial portfolio profile.

After profiling, the team may define a focused analytical subset for deeper work, for example:
- selected departments;
- selected grant schemes;
- selected recipient groups;
- selected geographies.

The subset must be reproducibly derived from the full frozen source.

## Recommended Analytical Grain

Model the data at the lowest reliable source grain, typically:
- award-level records;
- scheme-level records;
- recipient-level derived views.

Do not treat a scheme record and an award record as the same grain.

## Recipient Entity Resolution

Recipient names can vary.

If standardising recipient names:
- retain original recipient name;
- create a separate standardised field;
- maintain a match/exception log;
- never silently merge ambiguous recipients.

## Historical Extension

The core project can be completed from 2024–25 alone.

Optional:
- add earlier annual Grants Registers for multi-year concentration analysis.

Only do this after confirming comparable columns and definitions.

## Geographic Guidance

Use geography only where the source clearly defines what it represents.

Do not assume recipient address equals beneficiary or delivery location.

## File Size Guidance

The ODS is large enough to require care but is still suitable for the approved frozen source workflow.

If repository performance becomes poor:
- keep the raw ODS in approved shared storage;
- preserve a manifest and checksum in GitHub;
- keep reproducibly derived processed extracts in the team repository where suitable.

## Assessment Baseline

The project must be reproducible from the frozen 2024–25 register and the documented transformation logic.
