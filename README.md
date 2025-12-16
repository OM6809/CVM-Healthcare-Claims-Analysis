# CVM-Healthcare-Claims-Analysis
A comprehensive analysis of Syntegra’s Medicare CCLF (Claims) dataset focused on Cardio Vascular Metabolic (CVM) diseases. This repository answers key business questions involving claims trends, healthcare provider (HCP) prescribing behaviors, and patient age demographics. The insights will aid Sales &amp; Marketing leadership in refining strategies.
---

# CVM Claims Analysis – Medicare CCLF Data (2016–2018)

## Project Overview

This project was completed as part of **BIA-810D: Healthcare and Advanced Data Analytics (Fall 2025)**. It analyzes de-identified Medicare **CCLF claims data** from **Syntegra.io**, focusing on **Cardio Vascular Metabolic (CVM) diseases**.

Using **Part A** and **Part B (DME & Physician)** claims, the analysis uncovers trends in CVM procedures, healthcare provider behavior, patient demographics, and provides **actionable sales and marketing recommendations**.

---

## Objectives

* Quantify the share of CVM claims relative to total Medicare claims (2016–2018)
* Segment Healthcare Providers (HCPs) based on CVM claim volume
* Analyze CVM claim distribution across patient age groups
* Recommend data-driven strategies for sales force and marketing optimization

---

## Dataset Description

**Primary CSV files used:**

* `beneficiary_demographics.csv` – Patient demographics
* `parta_claims_header.csv` – Part A claim headers
* `parta_claims_revenue_center_detail.csv` – Revenue center details
* `parta_diagnosis_code.csv` – ICD diagnosis codes
* `parta_procedure_code.csv` – ICD procedure codes
* `partb_dme.csv` – Part B DME claims
* `partb_physicians.csv` – Part B physician claims

**Supporting files:**

* `Healthcare_Midterm_Analysis_Om_Final.html` – Additional methodology notes
* `Healthcare_Midterm_Om_Final.ipynb` – Primary analysis notebook
* `Healthcare_Midterm_Om_Finall.docx` – Final reports

---

## Business Questions

### CVM Trends

* What percentage of total claims are CVM-related each year?
* How should these trends influence sales and marketing strategy?

### HCP Segmentation

* How many providers fall into each CVM activity group?

  * Disease Aware (1 claim)
  * Trialists (2–4 claims)
  * Rising Stars (5–9 claims)
  * High-Volume Prescribers (10+ claims)
* How should engagement models differ by segment?

### Patient Demographics

* How are CVM claims distributed across age groups (18–59, 60–69, 70–79, 80+)?
* What are the year-over-year changes?

---

## Key Insights

* **CVM claims are increasing** as a share of total claims, indicating rising disease burden.
* **Disease Aware providers**, despite low CVM volume, contribute to high overall costs and represent growth opportunities.
* **High-Volume Prescribers** benefit most from brand-specific, in-person engagement.
* CVM claims are concentrated in **older populations (70+)**, while younger groups benefit from prevention-focused messaging.

---

## Technical Approach

* Merged multiple datasets using `claim_id` and `patient_id`
* Appended Part B DME and physician claims to Part A data
* Calculated patient age at time of claim
* Segmented HCPs based on CVM claim volume
* Aggregated results by year and age bucket

---

## Data Quality Checks

* Removed duplicate claim records
* Validated uniqueness of key identifiers
* Handled missing diagnosis and HCPCS codes
* Standardized date formats (YYYY-MM-DD)
* Converted numeric fields to appropriate data types

---

## Visualizations

* 100% stacked bar charts: CVM vs. non-CVM claims (2016–2018)
* HCP segmentation distribution by year
* Age-bucket distribution of CVM claims
* Year-over-year percentage change tables

---

## Future Work

* Map ICD codes to granular CVM subcategories
* Build predictive models to forecast CVM claim volume
* Identify high-cost CVM procedures
* Add geographic analysis for regional targeting

---

## Contact

**Author:** Om Rane
📧 **[orane@stevens.edu](mailto:orane@stevens.edu)**

---
Disclaimer: This analysis uses de-identified data from Syntegra. All references to real patients/providers are coincidental. This project is for educational purposes; any commercial or clinical application should undergo further validation and ethical review
