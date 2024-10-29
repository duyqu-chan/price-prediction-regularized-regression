# Regression with Regularization: Ridge, Lasso, and ElasticNet

This repository demonstrates the use of regularized regression models (Ridge, Lasso, and ElasticNet) for price prediction. We explore how regularization techniques can prevent overfitting and improve model interpretability through feature selection.

## Table of Contents
- [Overview](#overview)
- [Data Preparation](#data-preparation)
- [Models and Regularization](#models-and-regularization)
- [Evaluation Metrics](#evaluation-metrics)
- [Results and Findings](#results-and-findings)
- [Appendix](#appendix)

## Overview
In this project, we compare three regularized regression models—Ridge, Lasso, and ElasticNet—to predict prices based on various features. Regularization helps to penalize large coefficients, preventing overfitting and, in the case of Lasso and ElasticNet, enabling feature selection.

## Data Preparation
Data was preprocessed using `StandardScaler` to standardize features. This helps ensure fair regularization and avoids data leakage by fitting the scaler only on training data.

## Models and Regularization
- **Ridge Regression**: Applies L2 regularization, shrinking coefficients to reduce overfitting.
- **Lasso Regression**: Uses L1 regularization, which can set some coefficients to zero, aiding in feature selection.
- **ElasticNet Regression**: Combines L1 and L2 penalties, balancing feature selection with coefficient shrinkage.

## Evaluation Metrics
To evaluate each model, we use:
- **Mean Absolute Error (MAE)**
- **Mean Squared Error (MSE)**
- **Root Mean Squared Error (RMSE)**
- **R² Score**

These metrics help compare models’ performance in terms of prediction accuracy and variance explanation.

## Results and Findings
- **Lasso** performed best across all metrics, suggesting effective feature selection.
- **Ridge** performed comparably well, especially when retaining all features.
- **ElasticNet** did not outperform Lasso or Ridge, likely due to the combined penalties not offering additional benefit in this dataset.

## Appendix
The full `regression` function used in this project is available in the notebook under the appendix section.
