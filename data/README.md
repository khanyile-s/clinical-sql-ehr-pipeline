
# Clinical EHR Cohort Extraction & Population Health Analysis

### PostgreSQL | SQL | Clinical Informatics | Biomedical Data Science

## Overview

This project explores the application of relational database
management and SQL-based analytical methods to synthetic
Electronic Health Record (EHR) data.

Using PostgreSQL and the Synthea synthetic patient dataset,
this project develops a reproducible workflow for clinical
data preparation, disease-specific cohort extraction,
demographic characterization, comorbidity assessment,
and healthcare utilization analysis.

The project forms part of an ongoing computational
biomedical research portfolio focused on developing
quantitative skills at the intersection of biomedical
science, clinical informatics, and health data analytics.

## Research Objectives

- Develop a relational database for structured clinical data.
- Extract clinically defined patient cohorts using SQL.
- Characterize population demographics and clinical features.
- Investigate comorbidity and multimorbidity patterns.
- Explore healthcare utilization across patient subgroups.
- Develop reproducible analytical workflows for biomedical
  data research.

## Research Questions

1. What are the demographic characteristics of the
   synthetic patient population?

2. How can patients with chronic kidney disease (CKD)
   be identified and characterized using clinical records?

3. What chronic conditions commonly co-occur with CKD
   in the synthetic population?

4. How does healthcare utilization vary across
   disease-specific patient cohorts?

5. How can relational database techniques support
   reproducible clinical cohort identification?

## Dataset

| Attribute | Description |
|---|---|
| Source | Synthea Synthetic Patient Generator |
| Dataset | Synthetic Mass |
| Data type | Synthetic longitudinal EHR |
| Database | PostgreSQL |
| Coding systems | To be verified against source data |
| Privacy | No real patient data or PHI |

See [`data/README.md`](data/README.md) for details
on the dataset, data governance, and preparation.

## Technologies

| Technology | Application |
|---|---|
| PostgreSQL | Relational database management |
| SQL | Data extraction and analytical querying |
| Git & GitHub | Version control and documentation |
| Python | Planned statistical analysis and visualization |

## Project Structure

```text
clinical-ehr-cohort-analysis/
├── README.md
├── data/
│   └── README.md
├── sql/
│   └── README.md
├── docs/
├── analysis/
└── python/
```

## Analytical Workflow

1. Data source identification and preparation
2. Relational database schema design
3. Data quality assessment and validation
4. Demographic characterization
5. Clinical cohort extraction
6. Comorbidity analysis
7. Healthcare utilization analysis
8. Interpretation and visualization of findings

## Skills Demonstrated

**Database Management**
- Relational schema design
- Primary and foreign key constraints
- Data integrity and validation

**SQL & Data Analysis**
- Filtering and conditional logic
- Aggregate functions and grouping
- Multi-table relational joins
- Subqueries and Common Table Expressions
- Window functions and analytical queries

**Biomedical Research**
- Clinical cohort definition
- Population health analysis
- Clinical data interpretation
- Reproducible research practices

## Data Governance

All patient records used in this project are synthetically
generated through Synthea.

No real patient data, personally identifiable information,
or protected health information are used.

This project is intended for educational, research
training, and portfolio development purposes.
Findings from synthetic data are not intended to
represent real-world clinical populations.

## Future Development

- Extend clinical cohort definitions.
- Develop advanced SQL analytical queries.
- Integrate Python for exploratory data analysis.
- Produce statistical summaries and visualizations.
- Explore machine learning applications using
  appropriately defined clinical datasets.

## Author

Biomedical science graduate developing computational
skills in clinical data analytics, biomedical
informatics, and AI-driven research.

This project is part of a broader portfolio exploring
the integration of molecular biology, quantitative
methods, and computational biomedical science.

