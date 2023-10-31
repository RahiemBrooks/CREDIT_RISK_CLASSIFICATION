# Credit Risk Analysis

In this project, we delved into the world of machine learning to scrutinize a dataset comprising historical lending activities from a peer-to-peer lending services company. Our primary aim was to construct a reliable model capable of discerning the creditworthiness of potential borrowers.

## Overview of the Analysis
Our analysis revolved around various crucial factors, including the loan amount, interest rate, borrower's income, debt-to-income ratio, number of borrower's accounts, derogatory marks, and total debt. We split the dataset, which consisted of 77,536 data points, into training and testing sets. The `LogisticRegression` module from the `scikit-learn` library facilitated the development of the initial logistic regression model (Logistic Regression Model 1), which was then applied to the testing dataset.

To ensure balanced and unbiased data, we resampled the training set using the `RandomOverSampler` module from the `imbalanced-learn` library, resulting in an equal number of data points for both low-risk and high-risk loans.

## Results

# Logistic Regression Model 1

- Precision: 93% (Low-risk loans were predicted with 100% precision, while high-risk loans were predicted with 87% precision)
- Accuracy: 94% 
- Recall: 95% (The model had 100% recall in predicting low-risk loans and 89% recall in predicting high-risk loans)

# Logistic Regression Model 2

- Precision: 93% (Low-risk loans were predicted with 100% precision, while high-risk loans were predicted with 87% precision)
- Accuracy: 100% 
- Recall: 100%


## Summary

Logistic Regression Model 2 exhibits a more reliable performance with a higher accuracy and recall rate, which is essential in minimizing false negative results. Despite predicting slightly more false positives compared to the first model, its precision and accuracy make it a better choice for predicting high-risk loans.