# feature selection SVD vs. classical
Feature Selection Using Singular Value Decomposition (SVD) Compared to Classical Methods

## Overview
This project studies feature selection in high-dimensional industrial data using a linear-algebraic approach based on Singular Value Decomposition (SVD) and compares it with classical methods.
The main objective is to evaluate whether a purely geometric, model-free method can compete with traditional filter and wrapper feature selection techniques

## Feature Selection Methods

Mutual Information (Filter method)
Selects features based on statistical dependency with the class labels.

Recursive Feature Elimination (Wrapper method)
Uses Random Forest to iteratively remove less important features.

SVD-based Method (Algebraic approach)
Features are ranked based on their contribution to the dominant singular vectors of the data matrix, without using any learning model.

## Evaluation

A Logistic Regression classifier is trained on each selected feature subset.
Evaluation metrics:

Accuracy

F1-score

Feature selection time

Feature overlap between SVD and RFE is also analyzed using a Venn diagram

## Key Findings

RFE achieves the best predictive performance but has high computational cost.

SVD is extremely fast and stable under noise, but yields lower classification performance.

Mutual Information offers a balance between speed and accuracy.

Feature overlap between SVD and RFE is minimal, highlighting different selection perspectives
