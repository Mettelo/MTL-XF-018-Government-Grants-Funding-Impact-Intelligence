# MTL-XF-018 — Government Grants Portfolio, Funding Concentration & Programme Intelligence

**Mettelo Project Studio**  
**Project ID:** MTL-XF-018  
**Project Type:** Cross-Functional Grants & Programme Analytics · Team project · Production-style portfolio project  
**Client:** Confidential National Grants & Programme Directorate  
**Sector:** Public Sector / Grants / Programme Management  
**Engagement Type:** Simulated confidential-client engagement  
**Status:** Pre-launch  
**Recommended Team Size:** 6–8  
**Delivery Window:** 8 weeks  
**Master Repository:** Mettelo-controlled

> **Confidentiality Notice**  
> The client identity is intentionally withheld. This is a simulated Mettelo Project Studio engagement built around official public/open data. Participants must not represent the simulated client as a real external Mettelo customer.

## Challenge

Grant leaders oversee a large portfolio of schemes and awards but do not have one consistent view of recipient concentration, portfolio mix, multi-scheme recipients, geographic coverage and potential overlap. The organisation needs stronger evidence before the next funding cycle.

Your team will work as a multidisciplinary delivery team rather than as a group of people independently producing charts.

The engagement combines business analysis, data governance, data engineering, analytics, BI/decision support, assurance and specialist roles relevant to the project.

## Commissioned Decision

> **Where should grant-management teams investigate concentration, duplication, under-reach or portfolio imbalance before the next funding cycle?**

A successful submission must help structure or support this decision. A dashboard without governed definitions, reproducible data, analytical evidence and a defensible decision framework is not sufficient.

## Official Data Source

**Government Grants Register 2024–25 — scheme and award data**

Official publisher/source:

https://www.gov.uk/government/statistics/government-grants-statistics-2024-to-2025

The project uses a frozen Mettelo cohort copy/reference of the approved source wherever licensing and file-size rules permit. Teams should not depend on a live website or API remaining unchanged.

See:
- [Data workspace](data/README.md)
- [Source register](data/SOURCE_REGISTER.md)
- [Raw data folder](data/raw/)

## Core Objective

Build a reproducible cross-functional solution that:

1. build a governed scheme-award-recipient analytical model;
2. standardise recipient, department, scheme and award-value fields;
3. measure funding concentration by value and award count;
4. identify recipients appearing across multiple schemes;
5. assess portfolio mix and geographic coverage;
6. develop investigation flags for concentration, overlap and under-reach;
7. build portfolio decision-support BI;
8. complete entity-resolution assurance, UAT and handover;

## Key Business Questions

- Which recipients and schemes account for the largest share of funding?
- Where is funding concentrated among relatively few recipients?
- Which recipients appear across multiple schemes or departments?
- Which areas or programmes appear under-represented?
- What additional outcome evidence is required before making impact or value-for-money claims?

## Required Delivery Flow

```text
Discovery & stakeholder understanding
        ↓
Business requirements & acceptance criteria
        ↓
Data governance & source control
        ↓
Data ingestion & analytical modelling
        ↓
Data quality, reconciliation & exceptions
        ↓
KPI definition
        ↓
Core analysis
        ↓
Decision / prioritisation framework
        ↓
BI / decision-support product
        ↓
Assurance & UAT
        ↓
Executive recommendation
        ↓
Technical & operational handover
```

## Cross-Functional Team Model

The exact allocation can vary by team, but the project should demonstrate meaningful contribution across:

- Business Analysis;
- Data Governance;
- Data Engineering;
- Data Analysis / Domain Analysis;
- BI Development;
- Risk, Assurance or QA;
- specialist roles defined in the project brief;
- Data Science / AI or Model Governance where applicable.

One person may cover more than one function in a smaller team, but ownership and evidence must remain explicit.

## Minimum Delivery Standard

The final repository must demonstrate:

- traceable stakeholder requirements;
- governed metric and field definitions;
- frozen source/version documentation;
- reproducible data preparation;
- row/value reconciliation;
- explicit data-quality exceptions;
- project-specific analysis;
- transparent decision/prioritisation logic;
- governed BI measures;
- user acceptance testing;
- technical handover;
- visible GitHub collaboration;
- clear individual contribution evidence.

## Important Interpretation Rules

- Funding value is not evidence of impact, waste, fraud or recipient performance.
- Do not silently merge ambiguous recipient names.
- Potential overlap is not automatically duplicate funding.
- State clearly what geographic fields represent.
- Do not use awarded value as a proxy for programme effectiveness.

## Agreed Success Standard

The engagement is considered successful only when:

- the approved frozen source can be identified and obtained;
- curated outputs can be regenerated from code/instructions;
- material exclusions and data-quality issues are quantified;
- headline KPIs reconcile to the curated analytical model;
- analytical conclusions answer the commissioned business questions;
- decision rules and thresholds are visible and challengeable;
- at least five headline dashboard measures reconcile to underlying data;
- UAT and assurance evidence is present;
- each member's contribution can be evidenced;
- a reviewer can reproduce the team's core outputs without undocumented manual changes.

Detailed sign-off tests are defined in:

- [Acceptance Criteria](project/ACCEPTANCE_CRITERIA.md)
- [Deliverables](project/DELIVERABLES.md)

## Repository Purpose

This master repository is the official Mettelo source of truth for:

- project scope and challenge;
- business context;
- approved data/source information;
- governance requirements;
- deliverables;
- acceptance criteria;
- team repository standards;
- final submission instructions.

Teams use this repository as the specification. Their delivery work is completed in their own team repository under the Mettelo GitHub organisation.

## Repository Structure

```text
.
├── README.md
├── project/
│   ├── README.md
│   ├── PROJECT_BRIEF.md
│   ├── BUSINESS_CONTEXT.md
│   ├── DELIVERABLES.md
│   ├── ACCEPTANCE_CRITERIA.md
│   └── GOVERNANCE.md
├── data/
│   ├── README.md
│   ├── SOURCE_REGISTER.md
│   ├── raw/
│   ├── reference/
│   └── metadata/
└── submission/
    ├── README.md
    ├── TEAM_REPOSITORY_STANDARD.md
    ├── SUBMISSION_GUIDE.md
    └── FINAL_SUBMISSION_TEMPLATE.md
```

## Start Here

### 1. Understand the engagement
- [Project Brief](project/PROJECT_BRIEF.md)
- [Business Context](project/BUSINESS_CONTEXT.md)

### 2. Understand what must be delivered
- [Deliverables](project/DELIVERABLES.md)
- [Acceptance Criteria](project/ACCEPTANCE_CRITERIA.md)

### 3. Understand governance and data
- [Governance](project/GOVERNANCE.md)
- [Data Workspace](data/README.md)
- [Source Register](data/SOURCE_REGISTER.md)

### 4. Create the team delivery repository
- [Team Repository Standard](submission/TEAM_REPOSITORY_STANDARD.md)
- [Submission Guide](submission/SUBMISSION_GUIDE.md)
- [Final Submission Template](submission/FINAL_SUBMISSION_TEMPLATE.md)

## Team Submission Model

Each project team creates its delivery repository **under the Mettelo GitHub organisation**.

Recommended naming:

`MTL-XF-018-<team-name>`

The Team Lead adds every team member using their individual GitHub account.

Teams should use issues, branches, meaningful commits, pull requests and reviews where practical as evidence of collaborative delivery.

The team repository is the official delivery artefact. The master Mettelo repository remains the source of truth for the challenge specification.

## Final Review

The team presents to a Mettelo review panel acting as the simulated senior stakeholder group.

The panel may challenge:

- problem framing;
- requirements;
- data provenance;
- quality rules;
- metric definitions;
- analytical logic;
- thresholds;
- modelling assumptions;
- decision framework;
- dashboard usability;
- recommendations;
- limitations;
- reproducibility;
- contribution evidence.

A polished presentation does not compensate for weak evidence, unreproducible analysis or unclear ownership.

---
**Mettelo — Built for What’s Next**
