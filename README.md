# Clinical EHR Cohort Extraction & Analysis (PostgreSQL)

## Executive Summary
This project demonstrates end-to-end relational database querying and cohort extraction using synthetic Electronic Health Record (EHR) data generated via **Synthea**. The analytical pipeline focuses on filtering disease cohorts (such as Chronic Kidney Disease stages 1–4), executing population health aggregations, and joining patient demographic records with longitudinal care logs.

This repository serves as a foundational component of my quantitative health data portfolio, highlighting data engineering and database skills required for clinical research and healthcare analytics (e.g., NHS Band 5+ analytical roles and UK PhD programs).

---

## Data Source & Governance
* **Dataset:** Synthea™ Synthetic Mass Patient Generator.
* **Information Governance:** All patient profiles are 100% synthetically generated. No real patient data or protected health information (PHI) was used.
* **Clinical Coding:** Diagnosis data utilizes standard ICD-9/clinical classification codes.

---

## Key SQL Techniques Demonstrated
1. **Relational Schema Definition:** DDL table building for multi-relational health records.
2. **Clinical Subgroup Extraction:** Using `WHERE` and `IN` operators for disease-specific filtering.
3. **Epidemiological Aggregations:** Utilizing `GROUP BY` and `HAVING` logic to identify population health thresholds.
4. **Relational Joins:** Executing `LEFT JOIN` operations to integrate patient identity with clinical logs.

---

## Project Structure
```text
├── README.md                         <-- Project Documentation
└── queries/                          <-- SQL Analysis Scripts
