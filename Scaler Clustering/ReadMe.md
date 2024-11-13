# Scaler - Clustering Analysis for Job Profiles and Companies

## Problem Statement

Scaler is an online tech-versity that provides intensive computer science and data science courses. As part of the analytics vertical, the goal of this project is to profile the best companies and job positions for Scaler learners by clustering them based on their job profiles, companies, and other relevant features. This analysis aims to group learners with similar characteristics to derive actionable insights for Scaler.

### Data Dictionary
- **Unnamed 0**: Index of the dataset
- **Email_hash**: Anonymized Personal Identifiable Information (PII)
- **Company_hash**: Anonymized identifier for the current employer of the learner
- **orgyear**: Employment start date (year)
- **CTC**: Current Cost to Company (salary)
- **Job_position**: Job profile in the company
- **CTC_updated_year**: Year in which CTC was updated (for yearly increments or promotions)

## Concepts Used

- Manual Clustering
- Unsupervised Clustering (K-means, Hierarchical Clustering)

## Steps to Follow

1. **Data Import and Exploration**
   - Load the dataset and perform exploratory data analysis (EDA) to check its structure and characteristics.
   - Examine unique email hashes and the frequency of occurrence, recording observations and inferences.

2. **Data Cleaning and Preparation**
   - Check for missing values and prepare the data for KNN or Mean Imputation.
   - Remove special characters from the dataset using regular expressions.
   - Identify and drop duplicates in the dataset.

3. **Feature Engineering**
   - Create a new column for ‘Years of Experience’ by subtracting the employment start year (orgyear) from the current year.
   - Perform manual clustering based on the learner’s company, job position, and years of experience.
   - Generate a five-point summary of CTC (mean, median, max, min, count) based on company, job position, and years of experience.
   - Merge this summary with the original dataset and create flags indicating learners with CTC greater than the average for their company and job position.

4. **Classification and Analysis**
   - Create classification flags:
     - **Designation Flag**: Values [1, 2, 3] based on CTC comparisons.
     - **Class Flag**: Values [1, 2, 3] for job position comparisons.
     - **Tier Flag**: Values [1, 2, 3] for company-level comparisons.

5. **Querying Insights**
   - Identify:
     - Top 10 employees earning more than most in their company (Tier 1).
     - Top 10 employees in data science per company earning more than peers (Class 1).
     - Bottom 10 employees in data science per company earning less than peers (Class 3).
     - Bottom 10 employees earning less than most in their company (Tier 3).
     - Top employees with specific years of experience in each department (Tier X).
     - Top 10 companies based on their CTC.
     - Top 2 positions in each company based on CTC.

6. **Data Processing for Unsupervised Clustering**
   - Apply label encoding and one-hot encoding for categorical variables.
   - Standardize the data to prepare for clustering.

7. **Unsupervised Learning - Clustering**
   - Evaluate clustering tendency.
   - Utilize the Elbow method to determine the optimal number of clusters for K-means clustering.
   - Perform K-means clustering and hierarchical clustering (consider sampling for performance).

8. **Insights from Clustering**
   - Analyze the results of clustering to provide actionable insights and recommendations for Scaler regarding potential company partnerships and job positions to target for their programs.

## Conclusion

This clustering analysis aims to provide Scaler with a comprehensive understanding of the job market and help them tailor their offerings to better meet the needs of their learners. The insights gained from this project will enable Scaler to focus on strategic partnerships with companies that align with the career aspirations of their students.
