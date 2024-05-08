# Lending Club Case Study

## Table of Contents
* [Group Facilitator](#group-facilitators)
* [Brief Overview](#brief-overview)
  * [Problem Statement](#problem-statement)
  * [Objective](#objective)
  * [Analysis Steps Followed](#analysis-steps-followed)
* [Language and Library Used](#language-and-library-used)
* [Conclusions](#conclusions)


## Group Facilitators
* Rohit Gotecha
* Anant Joshi

## Brief Overview
### Problem Statement
The online loan marketplace company needs to reduce the loss and gain the better profit by its decision to provide loan to a applicant based on applicants promptness and his/her loan history or credit history.
### Objective
Through the EDA analysis of the given loan data set, need to derive the following
* To derive the driving factor (driving variables) behind the loan default
* The company can utilize these factors for its portfolio and risk assessments

The Solution in this repository provides the detailed exploratory data analysis on the provided loan data, summarises the key metrics and provides the recommendations.

### Analysis Steps Followed
* Importing Necessary Library
* Data Loading
* Checking Missing Value
*  Removing columns
* Removing Null columns
  - Removing same value columns:(If the column have same value in all rows, it will not useful)
  - Removing extra columns, Which are not require
  - Removing Missing Data columns where Missing data >= 60%
* Removing Rows
  - Removing Current status from loan_status column
  - Find the duplicate rows in data
* Standardising Values
  - Standardise units
    - Convert Loan date to datetime
    - Convert Int_rate column to Float
    - Convert funded amount and loan amount to float
    - Rounding of the values to two decimal places
    - Convert term column to int
  - Sorting columns in ascending order
  - Looking Outliers
    - Annual income have Outliers
    - Removing Outliers from Annual income
    - detailed outline for Outliers
  - Checking/Replacing/Updating Missing Values and Null values in dataset
    - Removing pub_rec_bankruptcies null values which are not useful
    - Around 1033 rows do not have Employment length values, maybe they are not doing job and doing own business so adding Employment length mode value
    - replacing 'Source Verifed' with 'Verified' because both meaning same as Verified 
  - Adding new columns
  - Final Loan dataset
* Segmentation Analysis
* Univariate Analysis
  - Ordered categorical data
  - Unordered categorical data
  - Quantitative variables
  - Summary of Univariate Analysis
* Bivariate Analysis
  - Ordered categorical data
  - Unordered categorical data
  - Quantitative variables
  - Summary of Bivariate Analysis
* Multivariate Analysis, Correlation Analysis
  - Heatmap for Multivariate Analysis, Correlation Analysis
  - Clustermap for Multivariate Analysis, Correlation Analysis
  - Summary of Multivariate Analysis, Correlation Analysis

## Language and Library Used
### Language
* Python
### Numerical Analysis and Data Analysis
* Numpy
* Pandas
### Data Visualization
* Seaborn
* MatplotLib-pyplot

## Conclusions
* Given that the majority of loans fall within the range of $5000 to $15000 and most interest rates range between 9% and 14%, the lending company should consider offering loans within these ranges to minimize the risk of defaults. Loans falling outside these ranges could be subject to closer scrutiny or higher interest rates.
* Since individuals with "Charged off" loans predominantly reside in rental properties, the lending company should assess the financial stability of applicants residing in rental properties more thoroughly. This could involve additional verification steps or adjustments to loan terms based on the applicant's housing situation.
* Applicants opting for longer loan terms, particularly 60-month terms, exhibit a higher percentage of charge-offs. Additionally, loans from Grades B, C, and D have a higher likelihood of being charged off. Therefore, the lending company should exercise caution when approving loans with longer terms or from lower-grade applicants, implementing stricter criteria or higher interest rates for such cases.
* Most borrowers have been in the workforce for ten years or more, and they are also the most likely to default on their loans.
* Borrowers who apply for loans with a 60-month term are at a higher risk of default compared to those who opt for a 36-month term loan.



