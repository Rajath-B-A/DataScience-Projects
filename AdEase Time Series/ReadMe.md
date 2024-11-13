# AdEase Time Series Forecasting

## Project Overview:

AdEase, an ads and marketing infrastructure company, aims to help businesses optimize ad placement by predicting page views on Wikipedia articles. Our goal is to leverage time series analysis to forecast the daily view count for 145,000 Wikipedia pages, enabling effective ad placement targeting specific regions and languages. This project covers 550 days of historical view data and incorporates significant events as exogenous variables for English pages.

## Data Dictionary
SPECIFIC NAME _ LANGUAGE.wikipedia.org _ ACCESS TYPE _ ACCESS ORIGIN: Page name format includes the article's title, language, access type (e.g., desktop, mobile), and access origin (e.g., spider, browser).
Exogenous variable (campaigns): Indicates impactful campaign dates, specifically for English pages.

## Project Steps
1. Data Import and Preprocessing -
Load datasets and check structure.
Clean and handle null values.
Split page name format to extract title, language, access type, and origin.
2. Exploratory Data Analysis (EDA) -
Analyze view count trends over time for different pages.
Visualize the distribution and trend of page views across languages, access types, and origins.
Draw insights regarding page popularity and access behavior.
3. Stationarity Check -
Test for stationarity using the Dickey-Fuller Test.
Perform time series decomposition.
Apply differencing to achieve stationarity if necessary.
Plot ACF and PACF to determine autoregressive and moving average parameters.
4. Modeling -
Build an ARIMA model to forecast page views.
Incorporate the exogenous campaign variable to develop a SARIMAX model for English pages.
Use Facebook Prophet to compare forecasting effectiveness across multiple models.
5. Forecasting -
Conduct forecasting across languages and regions, evaluating effectiveness of ad placements.
Test various model parameters to find the optimal fit.
6. Evaluation and Model Selection -
Use Mean Absolute Percentage Error (MAPE) to evaluate model accuracy (target range: 4-8%).
Employ grid search or alternative parameter selection techniques.
7. Inference & Recommendations -
Compare forecasts across languages and make recommendations for optimizing ad placements based on predicted page views.
Analyze results to determine the most effective forecasting model and parameters.

### Concepts Tested 
Exploratory Data Analysis (EDA)
Time Series Forecasting Techniques: ARIMA, SARIMAX, and Prophet
Model Evaluation & Optimization
