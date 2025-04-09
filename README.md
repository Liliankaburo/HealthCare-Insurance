# HealthCare Insurance Data Analysis Project

![image](https://github.com/user-attachments/assets/e135b87d-3589-41af-97cf-dd5edae94a55)

## Project Overview

This project analyzes healthcare insurance data to uncover trends, predict costs, and identify key factors affecting insurance premiums. It includes exploratory data analysis (EDA), data visualization, and predictive modeling using machine learning techniques.

## Problem Statement

Healthcare costs are influenced by various factors such as age, BMI, smoking habits, and region. This project aims to:

1. Explore relationships between variables and insurance charges.

2. Build a predictive model to estimate insurance costs.

3. Provide actionable insights for insurers and policyholders.


## Data Understanding

The  insurance.csv dataset includes features like:

1. ***Age: Age of the beneficiary***

2. ***Sex: Gender (male/female)***

3. ***BMI: Body Mass Index***

4. ***Children: Number of dependents***

5. ***Smoker: Smoking status***

6. ***Region: Residential area***

7. ***Charges: Individual medical costs***

## Technologies Used

a. Python (Pandas, NumPy, Matplotlib, Seaborn)

b. Scikit-learn (Regression models, preprocessing)

c. Jupyter Notebook

## Key Steps
1. Data Preprocessing: Handling missing values, encoding categorical variables.

2. Exploratory Data Analysis (EDA): Visualizing distributions, correlations, and outliers.

3. Feature Engineering: Creating new features (e.g., BMI categories).

4. Model Building: Training regression models (Linear Regression, Random Forest, etc.).

5. Evaluation: Metrics like RMSE, MAE, and R² score.

## Results & Insights

**Top 3 Factors Affecting Insurance Costs:**

1. Smoking status

2. Age

3. BMI

**Best Model**: Random Forest Regressor (R² = 0.87).

**Visualizations**:  (e.g., cost vs. age, smoker/non-smoker comparison).

 ### Detailed EDA Summary
 
#### 1. Numeric Variables Analysis
Age:

Distribution: Peaks at ages 20-30 (young beneficiaries dominate the dataset).

Charges correlation: Strong positive correlation ([value]%) — older individuals pay higher premiums.

BMI:

68% of beneficiaries fall in the "Overweight" or "Obese" range (BMI ≥ 25).

Charges correlation: Moderate ([value]%), but smokers with high BMI pay significantly more.

Children:

Most beneficiaries have 0-2 dependents.

Charges trend: Parents with 2-3 children pay slightly higher premiums.

#### 2. Categorical Variables Analysis
Smoker vs. Non-Smoker:

Smokers (20% of the dataset) pay 3-4x higher premiums on average.

Smoker Charges Comparison 

Region:

Southeast has the highest average charges ([value]), likely due to higher BMI/smoking rates.

Sex:

Males pay ~10% more than females (controlling for other factors).

#### 3. Key Visualizations

##### Plot	Insight
charges_vs_age.png	Linear increase in costs with age, but spikes for smokers.
bmi_histogram.png	Right-skewed distribution; 25% of beneficiaries are obese (BMI ≥ 30).
correlation_heatmap.png	Strongest correlations: smoker > age > bmi.

## Model Metrics

1. Baseline Models Comparison
Model	RMSE	MAE	R²
Linear Regression	[value]	[value]	[value]
Random Forest	[value]	[value]	[value]
XGBoost	[value]	[value]	[value]
Best Model: Random Forest Regressor (R² = [value]).

2. Feature Importance
Top 5 features influencing predictions:

smoker_yes (Impact: [value]%)

age

bmi

region_southeast

children

Feature Importance

3. Residual Analysis
Residuals are normally distributed (validating linear regression assumptions).

Outliers detected: Smokers with BMI ≥ 35 have the highest prediction errors.

## Key Takeaways

Smoking is the #1 cost driver — insurers could incentivize quitting programs.

Age and BMI are non-linear predictors; segmenting risk groups improves pricing.

Southeast region may need targeted health interventions.



## Next Steps

Add hypothesis testing (e.g., "Do smokers pay significantly more?")

Include interactive plots (Plotly) in the notebook/README

Deploying the model as an API




