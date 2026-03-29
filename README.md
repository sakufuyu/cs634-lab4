# MSCS_634_Lab_4

## Purpose
The purpose of this lab is to compare different regression models using the Diabetes Dataset from sklearn.

## Dataset
The Diabetes Dataset contains 442 samples and 10 features related to patient health. The goal is to predict disease progression.

## What I Did
I loaded the dataset, checked for missing values, and applied several regression models:
- Simple Linear Regression (one feature)
- Multiple Regression (all features)
- Polynomial Regression
- Ridge Regression
- Lasso Regression

## Results

Simple Linear Regression:
- R² ≈ 0.23

Multiple Regression:
- R² ≈ 0.45

Polynomial Regression:
- No improvement over simple regression

Ridge Regression:
- Best R² ≈ 0.46 (alpha = 0.10)

Lasso Regression:
- Best R² ≈ 0.47 (alpha = 0.10)

Although Lasso achieved the highest R², the difference compared to Ridge is minimal, suggesting similar overall performance.

## Key Insights
Using more features improved model performance. Polynomial regression did not help in this case. Regularization (Ridge and Lasso) improved the results slightly, and Lasso performed the best.

Polynomial regression did not improve performance, likely due to overfitting or lack of strong nonlinear relationships in the dataset.

Lasso slightly outperformed Ridge because it performs feature selection by reducing less important coefficients.

## Challenges / Decisions
I used one feature for simple and polynomial regression to keep the comparison clear. I tested several alpha values to observe how regularization affects performance. I avoided overly complex models to keep the analysis simple and clear.

The small performance differences between models indicate that simpler models may be sufficient for this dataset.