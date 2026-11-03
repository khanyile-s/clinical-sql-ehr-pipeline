
# Data Directory

## Overview

This directory is designated for the synthetic clinical dataset
used throughout the Clinical EHR Cohort Extraction & Analysis
project.

The dataset supports the development and execution of
relational database queries, clinical cohort identification,
and population health analyses using PostgreSQL.

## Data Source

**Synthea™ — Synthetic Patient Population Generator**

Synthea is an open-source synthetic patient generator that
produces realistic but artificial patient records, including
demographics, clinical encounters, conditions, medications,
procedures, and observations.

Dataset: Synthea Synthetic Mass (Massachusetts, USA)

Source: https://github.com/synthetichealth/synthea

## Data Governance & Privacy

- All patient records are synthetically generated.
- No real patient data are used.
- No personally identifiable information (PII) or protected
  health information (PHI) is included.
- Data are used exclusively for educational, analytical,
  and portfolio development purposes.

## Data Organization

Raw source files will be maintained separately from
analytical outputs wherever possible.

Expected source tables may include:

| File | Description |
|---|---|
| patients.csv | Synthetic patient demographics |
| encounters.csv | Longitudinal healthcare encounters |
| conditions.csv | Diagnoses and clinical conditions |
| observations.csv | Clinical measurements and observations |
| procedures.csv | Recorded clinical procedures |
| medications.csv | Medication records |

The availability of individual tables and fields depends
on the selected Synthea export configuration.

## Data Preparation

Before analysis, the dataset will undergo:

- Schema inspection and documentation
- Data type validation
- Missing-value assessment
- Duplicate record checks
- Relational integrity verification
- PostgreSQL import and validation

## Usage

Raw data files are not committed to this repository by default.

Users should download or generate their own Synthea dataset
following the official documentation and configure the
database locally.

This approach supports reproducibility while keeping
the repository lightweight.
