# Business Context

## Business Problem

The grants directorate manages a large number of schemes and awards across departments, recipients and geographies. Current reporting is good at showing total funding, but much weaker at answering whether the portfolio is becoming concentrated, whether the same recipients are repeatedly receiving funding across multiple schemes, or whether certain areas appear under-represented.

This creates a portfolio-management problem. High funding concentration may be entirely legitimate, apparent overlap may represent different programme objectives, and recipient location may not represent beneficiary location. Without a governed view, leadership cannot separate a useful investigation signal from an unsupported claim about waste, duplication or impact.

The business problem is to create a transparent grants-portfolio intelligence product that helps leadership identify where concentration, overlap, under-reach or data-quality issues deserve further review before the next funding cycle.

## Required Delivery Response

The team is expected to build a grants portfolio and funding-concentration decision-support solution.

The work should include:
- defining portfolio-review questions and stakeholder requirements;
- creating a governed scheme-award-recipient analytical model;
- standardising scheme, department, recipient and award-value fields;
- building an auditable recipient-name matching/entity-resolution process;
- calculating funding concentration by value and award count;
- identifying recipients appearing across multiple schemes or departments;
- analysing scheme mix and available geographic coverage;
- distinguishing potential overlap from proven duplication;
- documenting what outcome evidence would be required for impact/value-for-money analysis;
- building transparent investigation-priority rules and BI;
- completing reconciliation, entity-resolution assurance, UAT and handover.

## How the Client Will Use the Output

The finished product should support an annual portfolio review before future grant allocations are agreed. A Grants Director should be able to identify where a small number of recipients account for a large share of awards, see where recipients appear across multiple schemes, and decide whether the pattern requires further due diligence, programme coordination or no action.

The product must not present funding concentration as evidence of waste, fraud or poor programme impact.

## Client
**Confidential National Grants & Programme Directorate**

## Problem
Leadership oversees a large grants portfolio but lacks a consistent view of award concentration, recipient dependence, programme overlap and geographic distribution. Existing reporting focuses on totals rather than whether the portfolio is balanced, concentrated or aligned with strategic intent.

## Decision Owner
**Director of Grants Management**

## Stakeholders
Programme Portfolio Lead, Grants Operations Lead, Finance Business Partner, Policy & Evaluation Lead, Data Governance Lead, Risk & Assurance Lead, BI & Insight Lead

## Decision
**Where should grant-management teams investigate concentration, duplication, under-reach or portfolio imbalance before the next funding cycle?**

## Role Responsibilities
| Role | Required contribution |
|---|---|
| Business Analyst | Define portfolio-review decisions, stakeholder requirements and acceptance criteria. |
| Data Governance Analyst | Govern scheme/award/recipient definitions, entity resolution, lineage and DQ rules. |
| Data Engineer | Build reproducible ingestion and scheme-award-recipient model. |
| Programme/Data Analyst | Own concentration, portfolio-mix, recipient and geographic analysis. |
| BI Developer | Build grants-portfolio decision support and drill-down. |
| Evaluation Analyst | Separate funding-output evidence from genuine outcome/impact evidence. |
| Risk/Assurance Analyst | Challenge concentration thresholds, recipient matching and overlap interpretation. |

## Evidence Chain
**Requirement → governed definition → transformation → quality control → metric/analysis → decision insight → recommendation → UAT**
