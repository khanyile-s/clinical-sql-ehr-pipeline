
# Data Dictionary

## Overview

This document describes the structure, variables, and
relationships of the synthetic Electronic Health Record
(EHR) dataset used in this project.

The data dictionary will be updated following inspection
of the source CSV files and implementation of the
PostgreSQL relational schema.

## Data Source

Synthea Synthetic Mass dataset.

The dataset contains synthetic longitudinal patient
records representing demographics, clinical encounters,
diagnoses, observations, and other healthcare-related
information.

## Core Tables

### 1. Patients

| Variable | Description | Data Type |
|---|---|---|
| Id | Unique patient identifier | VARCHAR |
| BIRTHDATE | Patient date of birth | DATE |
| GENDER | Recorded gender | VARCHAR |
| RACE | Recorded race | VARCHAR |
| ETHNICITY | Recorded ethnicity | VARCHAR |
| CITY | Patient city | VARCHAR |
| STATE | Patient state | VARCHAR |

### 2. Encounters

| Variable | Description | Data Type |
|---|---|---|
| Id | Unique encounter identifier | VARCHAR |
| PATIENT | Associated patient identifier | VARCHAR |
| START | Encounter start date/time | TIMESTAMP |
| STOP | Encounter end date/time | TIMESTAMP |
| ENCOUNTERCLASS | Encounter classification | VARCHAR |
| DESCRIPTION | Encounter description | TEXT |

### 3. Conditions

| Variable | Description | Data Type |
|---|---|---|
| PATIENT | Associated patient identifier | VARCHAR |
| ENCOUNTER | Associated encounter identifier | VARCHAR |
| START | Condition onset date | DATE |
| STOP | Condition resolution date | DATE |
| CODE | Clinical condition code | VARCHAR |
| DESCRIPTION | Clinical condition description | TEXT |

## Relational Structure

The database is expected to contain relationships between
patients, encounters, and conditions.

- One patient may have multiple encounters.
- One patient may have multiple recorded conditions.
- An encounter may be associated with multiple conditions.
- Patient identifiers link demographic records to
  longitudinal clinical records.

Primary keys, foreign keys, and cardinality will be
confirmed during schema implementation.

## Data Validation

The following characteristics will be examined:

- Unique patient and encounter identifiers
- Missing or incomplete demographic information
- Valid date and timestamp formats
- Referential integrity between tables
- Consistency of clinical coding
- Duplicate and overlapping records

## Notes

Variable names and data types are provisional and based
on the expected Synthea CSV export structure.

The final documentation will reflect the actual dataset
after source file inspection and database import.
