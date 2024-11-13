# Jamboree Education: Graduate Admissions Prediction Using Linear Regression

## Project Overview
Jamboree Education, known for helping students achieve their academic goals, has launched a feature that predicts the likelihood of a student's admission to Ivy League institutions based on an array of academic and experiential factors. This analysis seeks to assist Jamboree by identifying key factors influencing graduate admissions and building a linear regression model to estimate admission probabilities.

## Dataset
Features:
Serial No.: Unique identifier for each row
GRE Scores: GRE score out of 340
TOEFL Scores: TOEFL score out of 120
University Rating: Institution rating out of 5
SOP Strength: Strength of Statement of Purpose, rated out of 5
LOR Strength: Strength of Letters of Recommendation, rated out of 5
Undergraduate GPA: Undergraduate GPA on a 10-point scale
Research Experience: Binary indicator (0 or 1) for research experience
Chance of Admit: Admission probability, between 0 and 1

## Project Steps
1. **Exploratory Data Analysis (EDA)**
Data Structure and Characteristics: Initial data inspection, including shape, data types, and null values.
Dropping Unique Identifier: The Serial No. column will be removed as it holds no predictive value for admissions.
Descriptive Statistics: Summary statistics to understand the distribution of each feature.
Distribution Analysis: Visualizations such as histograms and boxplots to identify distribution patterns across variables.
2. **Analyzing Variable Relationships**
Correlation Matrix: Calculate correlations among independent variables to gauge multicollinearity and highlight influential features.
Variable Interactions: Scatterplots and pair plots to explore how independent variables relate to each other and to the dependent variable (Chance of Admit).
3. **Model Building**: Linear Regression
Library: Using Statsmodels for interpretability and in-depth analysis.
Model Fitting: Building an initial linear regression model to predict Chance of Admit based on independent variables.
4. **Assumptions of Linear Regression**
To ensure a reliable model, linear regression assumptions are tested and validated:
* **Multicollinearity Check**: Variance Inflation Factor (VIF) scores for each predictor.
* **Residual Mean Check**: Mean of residuals close to zero for unbiased predictions.
* **Linearity Check**: Residual plots to check for random distribution.
* **Homoscedasticity Test**: Consistency in variance of residuals across fitted values.
* **Normality of Residuals**: Q-Q plots to assess residual normality.

5. **Model Evaluation**
**Metrics**:
  * Mean Absolute Error (MAE): Average magnitude of errors.
  * Root Mean Squared Error (RMSE): Square root of average squared prediction errors.
  * R² Score: Proportion of variance explained by the model.
  * Adjusted R² Score: Adjusted metric to account for the number of predictors.
    
6. **Insights and Recommendations**
Based on the analysis and model results:
* Factors Impacting Admission: Insights into the most significant features affecting admission probability.
* Actionable Suggestions: Recommendations for students and counselors to improve admission chances.
* Alternative Linear Regression Models: Exploration of variations in regression techniques for potentially improved predictions.

## Conclusion
The analysis provides Jamboree with a data-driven model to estimate admission probabilities, while also offering insights into how students can enhance their profiles based on identified influential factors.
