# Synthetic Student Dropout Dataset

## Overview
This synthetic dataset was created for the activity **“Supervised vs Unsupervised Learning”**.  
It simulates a university student dropout prediction scenario using demographic, academic, and financial variables.

## Number of records
- 500 rows
- 12 columns

## Variables
| Variable | Type | Description | Suggested range / values |
|---|---|---|---|
| student_id | Categorical / ID | Unique identifier for each student | S1000, S1001, ... |
| age | Numeric (integer) | Student age at admission | Mostly 16 to 30; includes outliers |
| gender | Categorical | Student gender | Male, Female, Other |
| place_of_origin | Categorical | City or place of origin | Barranquilla, Soledad, Cartagena, Santa Marta, Valledupar, Montería, Other |
| high_school_avg | Numeric (float) | Average high school grade | Normally 1.0 to 5.0; includes outliers |
| admission_test_score | Numeric (float/integer) | Admission exam score | Normally 0 to 100; includes outliers |
| first_semester_avg | Numeric (float) | First semester grade average | Normally 0.0 to 5.0; includes outliers |
| socioeconomic_level | Numeric (integer) | Socioeconomic level | 1 to 6 |
| scholarship | Categorical | Whether the student has a scholarship | Yes / No / null |
| loan | Categorical | Whether the student has a student loan | Yes / No |
| financial_aid | Categorical | Whether the student receives financial aid | Yes / No |
| dropout | Categorical (target) | Whether the student dropped out | Yes / No |

## How null values were introduced
Null values were intentionally added to simulate incomplete real-world institutional data:
- `admission_test_score`: around 5%
- `first_semester_avg`: around 6%
- `scholarship`: around 4%
- `place_of_origin`: around 3%

These null values represent missing records, incomplete forms, or unavailable information.

## How outliers were introduced
Outliers were intentionally added to simulate unusual or erroneous records:
- **age**: values such as 14, 33, 34, and 35
- **admission_test_score**: values such as -5, 110, and 120
- **high_school_avg**: values such as 0.4, 0.6, 5.7, and 5.8
- **first_semester_avg**: values such as -0.3 and 5.6

These values can be used to test data cleaning and preprocessing methods.

## Output variable
The target variable is:
- `dropout`
  - **Yes** = student dropped out
  - **No** = student did not drop out

## Notes
This dataset is synthetic and was generated for academic purposes only.  
It does not correspond to real students or real institutional records.
