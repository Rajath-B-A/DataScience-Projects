# Ola - Ensemble Learning for Driver Attrition Prediction

## Problem Statement

Recruiting and retaining drivers is a significant challenge for Ola, with high churn rates leading to increased costs and diminished morale within the organization. As Ola expands its driver base, it becomes critical to predict and mitigate driver attrition effectively. The goal of this project is to predict whether a driver will leave the company based on various attributes, such as demographics, tenure information, and performance history.

### Dataset Features

- **MMMM-YY**: Reporting Date (Monthly)
- **Driver_ID**: Unique ID for drivers
- **Age**: Age of the driver
- **Gender**: Gender of the driver (Male: 0, Female: 1)
- **City**: City code of the driver
- **Education_Level**: Education level (0: 10+, 1: 12+, 2: Graduate)
- **Income**: Monthly average income of the driver
- **Date Of Joining**: Joining date for the driver
- **LastWorkingDate**: Last date the driver worked
- **Joining Designation**: Driver's designation at the time of joining
- **Grade**: Driver's grade at the time of reporting
- **Total Business Value**: Total business value acquired by the driver in a month (negative values indicate cancellations/refunds)
- **Quarterly Rating**: Quarterly rating of the driver (1-5, higher is better)

## Concepts Tested

- Ensemble Learning (Bagging and Boosting)
- KNN Imputation for Missing Values
- Handling Imbalanced Datasets

## Steps to Follow

1. **Data Import and Exploration**
   - Load the dataset and check its structure and characteristics.
   - Convert date-like features to their respective data types.

2. **Data Cleaning and Preparation**
   - Check for missing values and prepare the data for KNN imputation, considering only numerical features.
   - Aggregate the data to remove multiple occurrences of the same driver, grouping by Driver ID.

3. **Feature Engineering**
   - Create a column indicating whether the quarterly rating has increased for each driver (1 if increased, else 0).
   - Create a target variable indicating if the driver has left the company (1 if the last working day is recorded).
   - Create a column indicating whether the monthly income has increased for each driver (1 if increased, else 0).

4. **Statistical Summary and Correlation Analysis**
   - Generate a statistical summary of the derived dataset.
   - Analyze correlation among independent variables to understand their interactions.

5. **One-Hot Encoding and Class Imbalance Treatment**
   - Perform one-hot encoding on categorical variables.
   - Address class imbalance in the target variable using appropriate techniques.

6. **Standardization of Training Data**
   - Standardize the features to ensure uniform scaling across the dataset.

7. **Model Building with Ensemble Learning**
   - Implement Ensemble Learning techniques, including Bagging and Boosting, with hyper-parameter tuning.
   - Evaluate model performance using a classification report and ROC AUC curve.

8. **Results Evaluation and Insights**
   - Assess model performance and provide actionable insights and recommendations for Ola to improve driver retention strategies.

## Conclusion

This analysis aims to empower Ola with predictive insights that can enhance driver retention, reduce churn, and optimize the recruitment process. The results will be presented in a straightforward manner, ensuring clarity for stakeholders with varying levels of data science knowledge.
