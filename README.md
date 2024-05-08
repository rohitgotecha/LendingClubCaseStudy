# Lending Club Case Study

## Table of Contents
* [Group Facilitator](#GroupFacilitators)
* [Brief Overview](#BriefOverview)
* [Technologies Used](#TechnologiesUsed)
* [Conclusions](#Conclusions)


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



## Technologies Used


## Conclusions


