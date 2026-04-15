# Automobile-Loan-Prediction

## Project Overview

This project focuses on predicting Automobile loan default risk for a financial institution. The main objective is to identify customers who are likely to default on their vehicle loan payments by using customer demographic data, loan information, employment details, and credit-related variables.

The project simulates a real-world credit risk use case where machine learning can support loan approval decisions, risk-based segmentation, and portfolio risk management.

## Business Problem

A financial institution is experiencing an increase in default cases in its vehicle loan portfolio. Since loan default directly affects profitability and capital efficiency, the company needs a data-driven approach to assess borrower risk before approval.

The key business question is:

> Can we predict which customers are more likely to default on their vehicle loan?

## Objective

The objectives of this project are to:

- Predict the probability of vehicle loan default
- Build a machine learning pipeline for credit risk classification
- Convert model output into practical business risk bands
- Support lending decisions such as approve, manual review, reduce credit limit, or reject

## Dataset

The dataset contains customer-level information related to vehicle loan applications. It includes variables such as:

- Customer income
- Loan amount
- Loan annuity
- Employment status
- Age
- Family information
- Housing information
- Credit bureau-related variables
- External score sources
- Default status

The target variable is: Default
Where
0 = Non-default customer
1 = Default customer

## Methodology

The project workflow includes:

Data loading and initial inspection
Missing value analysis
Data type correction
Feature engineering
Train-validation split
Preprocessing pipeline
Baseline model using Logistic Regression
Advanced model using XGBoost
Model evaluation using AUC, precision, recall, F1-score, and confusion matrix
Risk band assignment for business decision-making

## Models Used

Two main models were developed:

Logistic Regression
Logistic Regression was used as a baseline model because it is simple, interpretable, and commonly used in credit risk modeling.

XGBoost Classifier
XGBoost was used as the advanced model because it can capture non-linear relationships, handle complex feature interactions, and generally performs well on structured tabular data.

Evaluation Metrics
Since the dataset is imbalanced, accuracy alone is not enough. The project uses the following metrics:
ROC-AUC
Precision
Recall
F1-score
Confusion Matrix

*Recall is especially important because missing high-risk customers may lead to financial losses.
