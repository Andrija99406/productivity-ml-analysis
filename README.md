# Productivity Prediction using Behavioral Data

This project analyzes how behavioral and psychological factors relate to individual productivity and builds predictive models using both classical and machine learning approaches.

## Objective
To identify key drivers of productivity and evaluate how well different statistical models generalize to unseen data.

## Data
The dataset includes variables such as:
- Screen time (work/leisure)
- Stress level
- Sleep quality and sleep duration
- Mental wellness index
- Exercise activity
- Demographic and work-related features

## Methods
Models were built and compared using 10-fold cross-validation:
- Linear regression (baseline models)
- Feature selection and manual refinement
- Polynomial feature extension
- Ridge regression (to handle multicollinearity)
- Random Forest (non-linear benchmark)

## Key Result
- The best-performing model is **Ridge Regression**
- Test performance: **R² ≈ 0.88**, MAE ≈ 4.2
- Linear structure explains the data well; non-linear models did not significantly improve performance

## Main Findings
- Stress and screen time are consistently negative predictors of productivity  
- Mental wellbeing and sleep quality show positive associations  
- Relationships are largely linear within the observed range  

## Tools
R, caret, glmnet, randomForest, ggplot2, dplyr

## Conclusion
Simple regularized linear models outperform more complex non-linear approaches for this dataset, suggesting stable and interpretable relationships between behavior and productivity.
