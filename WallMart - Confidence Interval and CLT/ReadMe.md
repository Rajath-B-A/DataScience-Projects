# Walmart - Customer Purchase Behavior Analysis

## About Walmart

Walmart is an American multinational retail corporation that operates a chain of supercenters, discount departmental stores, and grocery stores. With over 100 million customers worldwide, Walmart aims to leverage customer purchase behavior insights to enhance its business strategies.

## Business Problem

The management team at Walmart seeks to analyze customer purchase behavior, specifically focusing on the purchase amount against customer gender and various other factors. They aim to determine if spending habits differ between male and female customers, particularly if women spend more on Black Friday than men.


### Data Dictionary
- **User_ID**: User ID
- **Product_ID**: Product ID
- **Gender**: Sex of the User (Male/Female)
- **Age**: Age in bins
- **Occupation**: Occupation (masked)
- **City_Category**: Category of the City (A, B, C)
- **StayInCurrentCityYears**: Number of years stayed in the current city
- **Marital_Status**: Marital Status
- **ProductCategory**: Product Category (masked)
- **Purchase**: Purchase Amount

## Analysis Steps

1. **Data Import and Exploration**
   - Load the dataset and conduct exploratory data analysis (EDA) to understand its structure and characteristics.
   - Check for null values and outliers using visualizations like boxplots and statistical methods (e.g., `describe()`, `isnull()`).

2. **Customer Spending Analysis**
   - Analyze the amount spent per transaction for all 50 million female customers and all 50 million male customers.
   - Calculate the average purchase amounts for both genders and derive conclusions.

3. **Confidence Interval Calculation**
   - Use the sample averages to calculate an interval within which the population average spending may lie.
   - Apply the Central Limit Theorem (CLT) to compute confidence intervals for female and male customer spending.
   - Experiment with different sample sizes to observe the distribution of mean expenses across genders.
   - Adjust the width of the confidence interval (90%, 95%, 99%) and report the observations.

4. **Comparison of Confidence Intervals**
   - Assess whether the confidence intervals for average spending between males and females overlap.
   - Analyze how Walmart can leverage these findings for strategic decision-making and improvements.

5. **Additional Analysis**
   - Perform similar analyses for married vs. unmarried customers.
   - Analyze spending habits based on age by creating bins for life stages: 0-17, 18-25, 26-35, 36-50, 51+ years.

## Recommendations and Action Items
- Based on the analysis, provide actionable insights for Walmart to enhance marketing strategies, inventory management, and customer engagement initiatives.
- Suggest targeted promotions for specific demographics based on spending behavior insights.

## Conclusion

This analysis aims to empower Walmart with a better understanding of customer spending behaviors across different demographics, enabling data-driven decisions to optimize sales and improve customer satisfaction.
