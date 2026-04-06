# AI Job Posting Trends (2019-2023):
A Data Science Case Study

## Project Overview
This project analyzes a dataset of 50,000 AI job postings to identify the key drivers of salary, the most in-demand skills, and how education and experience requirements cluster across the industry.

## Technical Stack
Language: Python 

Libraries: Pandas (Data Manipulation), Matplotlib & Seaborn (Visualization), Scikit-learn (Machine Learning)

Tools: Google Colab, GitHub 

## Key Phases of Analysis
1. Data Preprocessing & Feature Engineering

   Skill Tokenization: Converted raw text strings of "Required Skills" into cleaned Python lists.
   
   Encoding: Implemented One-Hot Encoding for technical skills and Ordinal Encoding for Education (1-4), Experience (1-4), and Remote work categories (1-3).
3. Statistical Inference (Hypothesis Testing)
   
   Methodology: Performed Bootstrap Resampling with 10,000 iterations to compare salary means.
   
   The Question: Does the most common skill (Linux) significantly impact the average salary?
   
   Findings: The 95% confidence interval for the difference in means was [-445.12, 813.99]. Since zero is included in this interval, we fail to reject the null hypothesis, suggesting that this specific skill alone does not guarantee a salary premium.
   
5. Machine Learning (K-Means Clustering)
   
   Objective: Grouped AI skills based on Education, Experience, and "Remoteness".
   
   Optimization: Used the Elbow Method to determine an optimal $k=6$ clusters.
   
   Insights: Identified a positive correlation between required education levels and professional experience across skill clusters.
   
## Results & Business Insights
Market Demand: Demand for AI experts is relatively uniform across the economy, though Healthcare, Telecommunications, and Manufacturing lead slightly.

Salary Landscape: Most AI roles offer salaries between 60k and 170k, with a median of approximately 115k.

Education: A Bachelor's or Master's degree is the standard requirement for the vast majority of AI postings.

## Limitations & Reflections
Selection Bias: The dataset source is unknown, which may impact how representative the findings are of the global AI market.

Measure Ranges: Many variables fall within narrow ranges, making strong correlations harder to detect
