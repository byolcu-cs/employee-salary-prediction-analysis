# Employee Salary Prediction Analysis

Statistical and machine learning analysis of posted salary drivers using company traits, location proxies, and technical skill indicators.

## Overview
This project examines how company characteristics, geographic location proxies, and technical skill requirements relate to posted salaries for analytics and technology roles. The analysis was designed to balance **interpretability** and **predictive performance** by combining an inference-focused regression framework with machine learning extensions.

## Project Objective
The goal was to quantify which factors are most strongly associated with salary differences in job postings, with particular focus on:
- company size
- company age
- location effects
- technical skills such as Python, AWS, Spark, and Excel

## Dataset
The analysis uses a cleaned working dataset derived from a Kaggle-hosted job-posting salary source. The final modeling file contains **742 rows and 22 columns**, including salary, firm characteristics, location fields, and binary technical skill indicators.

## Methods
The project includes both classical statistical modeling and machine learning:

- **Exploratory Data Analysis (EDA)**
- **OLS regression on log salary**
- **Nested model comparison**
- **Random Forest**
- **Shallow Neural Network**

Key modeling choices included:
- modeling salary on the **log scale** to reduce skew
- using a **quadratic effect for company size**
- treating skill mentions as binary indicators of job requirements
- comparing interpretable and nonlinear approaches

## Key Findings
- Salaries tend to increase with **company size**, but the effect shows **diminishing returns** at larger firms.
- **Python** and **AWS** requirements show positive salary associations after accounting for firm traits.
- **Excel** adds relatively little marginal information once stronger technical indicators are included.
- **Random Forest** outperformed OLS and the shallow neural network in predictive performance, suggesting meaningful nonlinearities and interactions in the data.
- Feature importance results indicated that **company age**, **company size**, and **Python requirement** were among the strongest predictors.

## Business Relevance
This project has practical implications for:
- **job candidates**, who can better understand how technical skills and firm characteristics affect compensation
- **hiring teams**, who can benchmark pay bands based on company scale, maturity, and required skills
- **educators and training programs**, who can align curriculum with labor market signals

## Repository Contents
- `reports/final-salary-report.pdf` — final written report
- `source/salary-analysis.Rmd` — source R Markdown file
- `data/updated-salary-data.csv` — working dataset used in the report
- `references/references.bib` — bibliography file

## Skills Demonstrated
- regression modeling
- model comparison
- feature interpretation
- machine learning
- salary and labor market analytics
- reproducible reporting in R Markdown
- business communication of analytical results

## Notes
This repository presents a graduate-level data analytics project in portfolio format. It highlights the final report, reproducible source file, dataset, and references used in the analysis.
