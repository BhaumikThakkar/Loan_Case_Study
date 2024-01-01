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

\- Higher probability of defaulting for applicants with house ownership
as \'RENT\'. - Increased likelihood of defaulting for loans used to
clear other debts. - Interest rates in the range of 13-17% correlate
with higher default rates. - Higher default rates for applicants with an
income range of \$31,201 - \$58,402. - Longer employment history (10+
years) is associated with a higher probability of default. - Loans with
terms of 36 months show a higher default rate. - Verification status and
the number of inquiries in the last 6 months impact default rates. -
Loans issued in later months of the year, especially December, show
higher default rates.

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
