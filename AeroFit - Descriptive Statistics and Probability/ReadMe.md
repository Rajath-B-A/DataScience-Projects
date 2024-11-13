# Aerofit Treadmill Customer Profiling and Market Analysis

## Project Overview:

Aerofit, a leading fitness equipment brand, aims to identify customer characteristics for each type of treadmill in their product line to better recommend products to new customers. This project uses descriptive statistics and probability analysis to understand the profile of customers purchasing Aerofit treadmills, focusing on insights such as customer demographics, usage patterns, and fitness level.

## Business Problem
Aerofit’s market research team seeks to build a customer profile for each treadmill model (KP281, KP481, and KP781) to identify if and how customer characteristics vary across products. This analysis aims to optimize product recommendations by targeting the right treadmill based on a customer’s profile.

## Dataset
The project uses customer data collected over three months on individuals who purchased a treadmill from Aerofit stores. Key features include:

## Feature	Description
Product Purchased	Treadmill model purchased: KP281, KP481, KP781
Age	Customer's age (in years)
Gender	Customer gender: Male/Female
Education	Years of formal education
Marital Status	Marital status: Single or Partnered
Usage	Expected weekly usage frequency
Income	Annual income (USD)
Fitness	Fitness rating on a 1-5 scale
Miles	Expected weekly miles

## Project Steps
1. **Data Import and Initial Analysis**
Import and inspect the dataset (shape, data types, missing values).
Convert categorical variables as needed.
Generate statistical summaries (mean, median, standard deviation).
Identify outliers with boxplots and summary statistics.
2. **Descriptive Analysis & Visualizations**
Perform univariate and bivariate analysis:
Univariate Analysis: Histogram, distplot, and countplot for each feature.
Bivariate Analysis: Boxplots to examine relationships between customer demographics and product purchased.
Heatmaps and pair plots to explore correlations between numerical features.
Insights on the impact of features like age, gender, and income on treadmill type.
3. **Probability Analysis**
Create two-way contingency tables and calculate:
Marginal Probability: E.g., what percent of customers purchased each treadmill model.
Conditional Probability: E.g., probability of a male customer purchasing a KP781 treadmill.
Generate business insights based on these probabilities and their implications.
4. **Customer Profiling**
Segment customers based on usage, fitness, and income to identify distinct profiles for each treadmill type.
Highlight trends and unique customer characteristics for KP281 (entry-level), KP481 (mid-level), and KP781 (advanced) treadmills.
5. **Recommendations**
Actionable, non-technical recommendations for marketing, product positioning, and customer engagement.
