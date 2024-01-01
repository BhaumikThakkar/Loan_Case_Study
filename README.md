# Loan Default Analysis

This repository contains an analysis of loan data to identify factors
associated with loan defaulting. The analysis focuses on user details
and determining factors before loan approval. Below is a summary of the
key steps and findings:

## Data Import and Initial Exploration

The analysis begins by importing necessary libraries and loading the
loan data from a CSV file named \"loan.csv\". The dataset is explored
for null values and irrelevant columns.

## Data Cleaning

Several columns with exclusively null values or containing a single
value are removed to enhance the dataset\'s relevance. Columns related
to the post-approval phase of the loan are eliminated, narrowing down to
48 columns of interest.

## Handling Missing Values

Columns with missing values, specifically \"emp_length\" and
"revol_util,\" are addressed. The \"emp_length\" column is imputed with
the mode value, and rows with missing values in \"revol_util\" are
dropped.

## Standardizing the Data

Certain columns like \"revol_util,\" \"int_rate,\" and \"emp_length\"
are standardized to ensure consistency and ease of analysis.

## Outlier Treatment

Outliers in the \"annual_inc\" column are identified and removed,
ensuring a more accurate representation of the data.

## Visualizing Categorical Data

Categorical variables such as loan status, grade, subgrade, home
ownership, purpose, and others are visualized to gain insights into the
distribution of charged-off loans.

## Analysis of Loan Defaulting

The analysis identifies factors associated with a higher probability of
loan defaulting. Some key observations include:

- Applicants taking loan for 'home improvement' and have income of 60k -70k
- Applicants whose home ownership is 'MORTGAGE and have income of 60-70k
- Applicants who receive interest at the rate of 21-24% and have an income of 70k-80k
- Applicants who have taken a loan in the range 30k - 35k and are charged interest rate of 15-17.5 %
- Applicants who have taken a loan for small business and the loan amount is greater than 14k
- Applicants whose home ownership is 'MORTGAGE and have loan of 14-16k
- When grade is F and loan amount is between 15k-20k
- When employment length is 10yrs and loan amount is 12k-14k 
- When the loan is verified and loan amount is above 16k
- For grade G and interest rate above 20%

## Annual Income Analysis

The analysis explores the relationship between annual income and loan
defaulting. Insights include:

\- Annual income vs. loan purpose reveals varying preferences for
different income groups. - Homeowners with higher incomes tend to apply
for loans related to home improvement, house, renewable energy, and
small businesses.

## Loan Amount Analysis

The analysis delves into factors influencing loan amounts and their
relation to defaulting. Key observations include:

\- Higher loan amounts correlate with higher interest rates, longer
employment history, and verified loans. - The interest rate is
significantly higher for charged-off loans across all loan amount
groups.

## Conclusion

The analysis provides valuable insights into the factors influencing
loan defaulting, enabling better risk assessment and decision-making in
the lending process. Further analysis and modeling could enhance
predictive capabilities for identifying potential defaults.
