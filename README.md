# Annual Medical Cost Predictor

**DATASCI 347 Final Project**  
Isobel Li, Ria Krishna, Rishi Khullar, Ryana Rajesh

## Project Overview

This project uses machine learning models to predict annual medical costs using patient demographic information, lifestyle factors, health conditions, and healthcare utilization data. The goal was to better understand which factors contribute most strongly to healthcare spending and evaluate how well different predictive models perform on this task.

## Dataset

- Source: Kaggle (CDC + NIH sourced data)
- 100,000 patient observations
- 54 variables

### Features Included
- Demographics (age, income, BMI, education, region, etc.)
- Lifestyle factors (smoking, alcohol use)
- Health conditions (diabetes, asthma, cancer history, etc.)
- Healthcare utilization metrics

### Target Variable
- `annual_medical_cost`

## Models Used

- Linear Regression
- Bagging
- Random Forest
- Gradient Boosting

## Methods

- Exploratory data analysis (EDA)
- Log transformation of target variable
- Feature selection using correlation analysis
- Model evaluation using:
  - R²
  - RMSE
  - 5-fold cross validation

## Results

| Model | R² | RMSE |
|---|---|---|
| Linear Regression | 0.213 | 0.752 |
| Bagging | 0.196 | 0.760 |
| Random Forest | 0.212 | 0.752 |
| Gradient Boosting | 0.216 | 0.751 |

Gradient Boosting performed slightly better overall, though all models showed relatively similar predictive performance.

## Key Findings

Important predictors of annual healthcare cost included:
- Number of chronic conditions
- Hospitalization history
- Smoking status
- Age

The modest R² values suggest that healthcare cost prediction is highly complex and influenced by additional factors not fully captured in the dataset.

## Conclusion

This project demonstrates both the potential and limitations of machine learning for healthcare cost prediction. While predictive performance remained modest, the models provided useful insight into the patient characteristics most strongly associated with increased healthcare spending.

## Repository Contents

- `README.md` — project overview
- Documentation containing final report
- Powerpoint presentation with visualizations
- Full project code
- Raw dataset