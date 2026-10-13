# WHO Life Expectancy — Regression Analysis in R

## Project Overview

This project investigates life expectancy using linear regression and robust regression in R. It compares a supplied preprocessed dataset with the corresponding raw dataset and evaluates model performance on training and test sets.

The project was completed as part of **Advanced Methods for Regression and Classification at TU Wien**.

## Objectives

- Fit ordinary multiple linear regression models.
- Compare training and test performance using RMSE.
- Visualize measured versus predicted life expectancy.
- Interpret regression coefficients and statistical significance.
- Investigate multicollinearity using variance inflation factors (VIF).
- Examine model assumptions using diagnostic plots.
- Compare ordinary linear regression with robust regression.

## Tools and Technologies

- R
- RStudio
- R Markdown
- `lm()` for ordinary linear regression
- `lmrob()` from `robustbase` for robust regression
- Statistical diagnostics and data visualization

## Key Results

On the selected train/test split, the two ordinary linear regression models achieved nearly identical test RMSE values of approximately **3.55 years**.

The robust models did not improve test-set RMSE in this experiment. The robust model fitted to the raw data also produced a near-singularity warning, which is an important limitation when interpreting its results.

The analysis additionally identified multicollinearity among several predictors and deviations from some standard regression assumptions.

## Repository Contents

- `Exercise1_Karun_Krishnan.Rmd` — R Markdown source
- `Regression_Exercise_1_Report.pdf` — rendered report
- `figures/` — optional plots, if included

## How to Reproduce

1. Install R and RStudio.
2. Install the required R packages, including `robustbase` and `rmarkdown`.
3. Place the permitted input datasets in the project directory.
4. Open the `.Rmd` file in RStudio.
5. Knit the document to reproduce the report.

The original dataset files are not included in this repository. Use the authorized course-provided data files.

## Learning Outcomes

This project provided practical experience in regression modelling, predictive evaluation, coefficient interpretation, multicollinearity assessment, residual diagnostics, and robust statistical methods.

## Author

Karun Krishnan

*Academic project — TU Wien.*
