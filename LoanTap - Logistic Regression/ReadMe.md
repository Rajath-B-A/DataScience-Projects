# LoanTap Logistic Regression: Creditworthiness Assessment

## Context

LoanTap is an innovative online platform that offers customized loan products to millennials. By providing instant and flexible loans under consumer-friendly terms, LoanTap serves salaried professionals and businessmen. The data science team is focused on building an underwriting layer to evaluate the creditworthiness of individuals applying for personal loans.

## Problem Statement

The objective of this case study is to determine whether a credit line should be extended to an individual based on a set of attributes. Additionally, the project aims to recommend suitable repayment terms for the approved loans.

### Data Dictionary

- **loan_amnt**: Amount of the loan applied for by the borrower.
- **term**: Number of payments on the loan (in months, either 36 or 60).
- **int_rate**: Interest rate on the loan.
- **installment**: Monthly payment owed by the borrower.
- **grade**: Loan grade assigned by LoanTap.
- **sub_grade**: Loan subgrade assigned by LoanTap.
- **emp_title**: Job title supplied by the borrower.
- **emp_length**: Employment length in years (0-10).
- **home_ownership**: Home ownership status.
- **annual_inc**: Self-reported annual income of the borrower.
- **verification_status**: Status of income verification (verified, not verified).
- **issue_d**: Month the loan was funded.
- **loan_status**: Current status of the loan (Target Variable).
- **purpose**: Category for the loan request.
- **title**: Title provided by the borrower for the loan.
- **dti**: Debt-to-Income ratio.
- **earliest_cr_line**: Month the earliest credit line was opened.
- **open_acc**: Number of open credit lines.
- **pub_rec**: Number of derogatory public records.
- **revol_bal**: Total revolving balance.
- **revol_util**: Revolving line utilization rate.
- **total_acc**: Total number of credit lines.
- **initial_list_status**: Initial listing status of the loan (W, F).
- **application_type**: Indicates if the application is individual or joint.
- **mort_acc**: Number of mortgage accounts.
- **pub_rec_bankruptcies**: Number of public record bankruptcies.
- **Address**: Address of the individual.

## Concepts Used
- Exploratory Data Analysis (EDA)
- Feature Engineering
- Logistic Regression
- Precision vs. Recall Tradeoff

## Steps to Follow

1. **Data Import and Exploration**
   - Import the dataset and examine its structure and characteristics.
   - Analyze the target variable (`Loan_Status`) and its relationship with predictor variables using various plots (count plots, box plots, heatmaps).

2. **Feature Engineering**
   - Create flags for certain variables:
     - `Pub_rec`: 1 if > 1, else 0
     - `Mort_acc`: 1 if > 1, else 0
     - `Pub_rec_bankruptcies`: 1 if > 0, else 0
   - Handle missing values and treat outliers appropriately.
   - Normalize or standardize numerical features using MinMaxScaler or StandardScaler.

3. **Model Building**
   - Use the Logistic Regression model from the Sklearn/Statsmodel library to fit the data.
   - Evaluate the model results using:
     - Classification report
     - ROC AUC curve
     - Precision-recall curve

4. **Model Evaluation and Insights**
   - Analyze the precision-recall tradeoff to balance between detecting real defaulters and minimizing false positives.
   - Discuss the implications of non-performing assets (NPA) and the importance of cautious loan disbursement.

5. **Actionable Insights and Recommendations**
   - Provide clear, actionable recommendations based on the analysis and results of the logistic regression model.

## Conclusion

The LoanTap Logistic Regression project aims to create a robust underwriting process for personal loans, enabling LoanTap to extend credit lines judiciously while maximizing opportunities for responsible lending.
