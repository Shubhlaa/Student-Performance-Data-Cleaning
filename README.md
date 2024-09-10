# Student Performance Data Cleaning

# Project Overview
This project involves cleaning and preparing a dataset to analyze student performance in two Portuguese public schools: Gabriel Pereira (GP) and Mouzinho da Silveira (MS). The dataset contains student grades, background information, study time, and participation in extracurricular activities. The objective is to clean the data to ensure accuracy and completeness for further analysis to identify factors that impact student grades.

# Key Steps

## 1. Data Sorting
**Objective:** Identify potential data issues.
- Sorted the data by school (GP and MS) and age.
- Discovered students over 19 years old, which is beyond the valid high school age range (15-19 years).

## 2. Removing Incorrect Data
**Objective:** Remove inaccurate records.
- Filtered and deleted rows where students’ ages were 20, 21, and 22, following consultation with the superintendent.

## 3. Filling Missing Data
**Objective:** Ensure completeness in the `reason` column.
- Filtered the `reason` column, which explains why students chose a school.
- Filled missing values with `none_given`.

## 4. Converting Data for Analysis
**Objective:** Transform text data into numeric format.
- Converted non-numeric values in the `Medu` and `Fedu` columns (mother's and father's education levels) to numeric codes using the following mapping:
  - `none` → `0`
  - `primary education (4th grade)` → `1`
  - `5th to 9th grade` → `2`
  - `secondary education` → `3`
  - `higher education` → `4`

# Results
The dataset is now clean and ready for analysis, allowing exploration of factors that affect student performance, such as parental education levels, study time, and extracurricular participation.
