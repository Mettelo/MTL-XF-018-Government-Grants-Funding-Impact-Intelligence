# Project Brief

## Engagement Details
| Field | Detail |
|---|---|
| Project ID | MTL-XF-018 |
| Project Title | Government Grants Portfolio, Funding Concentration & Programme Intelligence |
| Client | Confidential National Grants & Programme Directorate |
| Sector | Public Sector / Grants / Programme Management |
| Duration | 8 weeks |
| Recommended Team Size | 6–8 |
| Primary Sponsor | Director of Grants Management |
| Senior Stakeholders | Programme Portfolio Lead, Grants Operations Lead, Finance Business Partner, Policy & Evaluation Lead, Data Governance Lead, Risk & Assurance Lead, BI & Insight Lead |
| Primary Dataset | Government Grants Register 2024–25 — scheme and award data |

## 1. Client Situation
Leadership oversees a large grants portfolio but lacks a consistent view of award concentration, recipient dependence, programme overlap and geographic distribution. Existing reporting focuses on totals rather than whether the portfolio is balanced, concentrated or aligned with strategic intent.

## 2. Business Decision
> **Where should grant-management teams investigate concentration, duplication, under-reach or portfolio imbalance before the next funding cycle?**

## 3. Agreed Objectives
1. Create a governed grant-scheme/award/recipient analytical model.
2. Standardise recipient, scheme, department and award-value fields with explicit exception rules.
3. Measure funding concentration, recipient dependence, programme mix and geographic reach without equating funding volume with impact.
4. Create a portfolio-review framework for concentration, overlap and under-reach.
5. Provide decision support for grants leadership, finance and evaluation teams.

## 4. Key Business Questions
1. Which recipients and schemes account for the largest share of awarded value?
2. Where is funding highly concentrated among a small number of recipients?
3. Which recipients appear across multiple schemes or departments?
4. Which programmes/geographies appear under-represented relative to the available portfolio data?
5. Which apparent overlaps may reflect legitimate multi-programme funding rather than duplication?
6. What additional outcome data would be needed before making impact or value-for-money claims?

## 5. Cross-Functional Roles
| Role | Minimum expected output |
|---|---|
| Business Analyst | Define portfolio-review decisions, stakeholder requirements and acceptance criteria. |
| Data Governance Analyst | Govern scheme/award/recipient definitions, entity resolution, lineage and DQ rules. |
| Data Engineer | Build reproducible ingestion and scheme-award-recipient model. |
| Programme/Data Analyst | Own concentration, portfolio-mix, recipient and geographic analysis. |
| BI Developer | Build grants-portfolio decision support and drill-down. |
| Evaluation Analyst | Separate funding-output evidence from genuine outcome/impact evidence. |
| Risk/Assurance Analyst | Challenge concentration thresholds, recipient matching and overlap interpretation. |

## 6. Minimum Delivery Standard
Traceable requirements; governed definitions/lineage; preserved raw data; reproducible transformation; reconciliation; project-specific analysis; transparent decision logic; governed BI; UAT; handover; collaborative evidence.

## 7. Constraints
- Award value is not evidence of impact, waste, fraud or recipient performance.
- Recipient-name standardisation can create false matches and must be auditable.
- Geographic fields may be incomplete or refer to recipient location rather than beneficiary location.
- Programme overlap is not automatically duplication.
- Impact/effectiveness conclusions require outcome data not contained in the grants register.

## 8. Agreed Success Criteria
- Award totals reconcile to the selected source scope after quantified exclusions.
- Recipient-name standardisation preserves a match log and never silently merges ambiguous entities.
- At least one concentration metric is calculated both by value and award count.
- Potential overlap flags are labelled for investigation and are not described as duplication without supporting evidence.
- No dashboard or briefing uses funding value as a proxy for programme impact.
- Geographic analysis states whether geography represents recipient, delivery or another available location concept.

## 9. Out of Scope
Core delivery excludes confidential personal data, paid production infrastructure, automated operational decisions and unsupported causal inference.

## 10. Reproducibility Definition
A reviewer should be able to clone the team repository, obtain the approved source data, execute the workflow and reproduce curated outputs and validation evidence without undocumented manual changes.
