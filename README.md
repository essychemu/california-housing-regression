# California Housing Regression Analysis

## Project Overview

This project analyzes the California Housing dataset using Python and statistical regression techniques. The analysis investigates how median income, average rooms, and average occupancy are associated with median house values.

## Objectives

* Build a multiple linear regression model.
* Evaluate model performance using R² and Adjusted R².
* Identify statistically significant predictors using p-values.
* Calculate 95% confidence intervals.
* Add a quadratic term to investigate a nonlinear relationship.
* Compare the base and quadratic regression models.

## Tools & Libraries

Python | Pandas | NumPy | Statsmodels | Scikit-learn | SciPy | Matplotlib | Seaborn

## Regression Analysis

The base model used three predictors:

* `MedInc` — Median Income
* `AveRooms` — Average Number of Rooms
* `AveOccup` — Average Occupancy

### Base Model Results

* **R²:** 0.4808
* **Adjusted R²:** 0.4807

The model explains approximately **48.08%** of the variation in median house values based on the selected predictors.

### Statistical Significance

The p-values for the model coefficients were:

| Coefficient | P-value |
| ----------- | ------: |
| Intercept   | 0.00000 |
| MedInc      | 0.00000 |
| AveRooms    | 0.00000 |
| AveOccup    | 0.00000 |

All four coefficients had p-values below the 0.05 significance level.

### 95% Confidence Intervals

| Coefficient | Lower | Upper |
| ----------- | ----: | ----: |
| Intercept   |  0.58 |  0.64 |
| MedInc      |  0.43 |  0.44 |

## Quadratic Regression

A new variable, `MedInc_squared`, was created by squaring `MedInc`:

`MedInc_squared = MedInc²`

The quadratic model produced:

* **R²:** 0.4858
* **Adjusted R²:** 0.4857

## Model Comparison

| Model           |     R² | Adjusted R² |
| --------------- | -----: | ----------: |
| Base Model      | 0.4808 |      0.4807 |
| Quadratic Model | 0.4858 |      0.4857 |

Adding the quadratic income term increased R² from **0.4808 to 0.4858** and Adjusted R² from **0.4807 to 0.4857**.

## What I Learned

Through this project, I learned how to:

* Build multiple linear regression models using Statsmodels.
* Prepare predictors and add an intercept.
* Interpret R² and Adjusted R².
* Use p-values to assess statistical significance.
* Calculate and interpret 95% confidence intervals.
* Create quadratic terms to model nonlinear relationships.
* Compare regression models using Adjusted R².
* Apply statistical analysis to a real-world housing dataset.

## Conclusion

This project demonstrates practical skills in Python-based data analysis, regression modeling, statistical inference, and model evaluation. The comparison between the base and quadratic models shows how adding a nonlinear term can change model performance.

