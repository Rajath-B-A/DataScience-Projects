# Yulu - Demand Analysis for Shared Electric Cycles

## About Yulu

Yulu is India’s leading micro-mobility service provider, offering unique vehicles for daily commutes. The company's mission is to eliminate traffic congestion in India by providing safe, user-friendly commuting solutions through a mobile app. Yulu zones are strategically located at metro stations, bus stands, office spaces, and residential areas to ensure smooth, affordable, and convenient transportation.

## Business Problem

Yulu has experienced significant dips in its revenues and has contracted a consulting company to investigate the factors affecting the demand for shared electric cycles in the Indian market. The objective is to identify the significant variables that predict demand and understand how well these variables describe the demand for electric cycles.

### Data Dictionary

- **datetime**: Datetime of the observation
- **season**: Season (1: spring, 2: summer, 3: fall, 4: winter)
- **holiday**: Whether the day is a holiday (1: Yes, 0: No)
- **workingday**: Whether the day is a working day (1: Yes, 0: No)
- **weather**: Weather conditions
  - 1: Clear, few clouds, partly cloudy
  - 2: Mist + cloudy, mist + broken clouds, mist + few clouds
  - 3: Light snow, light rain + thunderstorm + scattered clouds
  - 4: Heavy rain + ice pellets + thunderstorm + mist, snow + fog
- **temp**: Temperature in Celsius
- **atemp**: Feeling temperature in Celsius
- **humidity**: Humidity percentage
- **windspeed**: Wind speed
- **casual**: Count of casual users
- **registered**: Count of registered users
- **count**: Total rental bikes (casual + registered)

## Analysis Steps

1. **Data Import and Exploration**
   - Load the dataset and conduct exploratory data analysis (EDA) to understand its structure and characteristics.
   - Visualize relationships between dependent (count) and independent variables (working day, weather, season, etc.).

2. **Hypothesis Testing**
   - Establish hypotheses:
     - **Null Hypothesis (H0)**: There is no significant effect of the independent variable on the demand for electric cycles.
     - **Alternate Hypothesis (H1)**: There is a significant effect of the independent variable on the demand for electric cycles.
   - Conduct the following tests:
     - **Two-sample t-test** to assess the impact of working days on electric cycle rentals.
     - **ANOVA** to compare the number of cycles rented across different seasons.
     - **Chi-square test** to check the relationship between weather conditions and seasons.

3. **Assumption Checking**
   - Check the assumptions of the tests (normality, equal variance) using visual methods (histograms, Q-Q plots) and statistical methods (Levene’s test, Shapiro-Wilk test).
   - Proceed with analysis even if some assumptions fail, but note this in the reporting.

4. **Significance Level and Test Statistics**
   - Set a significance level (α), commonly 0.05.
   - Calculate test statistics for each hypothesis test and make decisions to accept or reject the null hypothesis.

5. **Inference from Analysis**
   - Interpret the results and draw conclusions regarding the factors affecting the demand for shared electric cycles in the Indian market.

## Recommendations and Action Items
- Based on the analysis, provide actionable insights for Yulu to enhance demand forecasting and improve service offerings.
- Suggest strategies to leverage significant factors for marketing and operational decisions.

## Conclusion

This analysis aims to empower Yulu with a deeper understanding of the variables influencing the demand for shared electric cycles, enabling data-driven decisions to enhance service utilization and revenue.
