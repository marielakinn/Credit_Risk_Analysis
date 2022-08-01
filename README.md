# Credit Risk Analysis

## Overview of the Project and Purpose

The purpose of this project is to utilize Machine Learning alogarithms and techniques to build and evaluate models using resampling.

The following will be achieved using the credit card credit dataset from LendingClub:

1. Oversample the data using the RandomOverSampler and SMOTE algorithms, and undersample the data using the ClusterCentroids algorithm
2. Use a combinatorial approach of over- and undersampling using the SMOTEENN algorithm
3. Compare two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk

## Results

### 1. Naive Random Oversampling

![](Resources/Capture1.PNG)

- Balanced Accuracy: 0.6612700484668286
- Precision: The precision is low for High-risk loans and is high for Low-risk loans.
- Recall: High/Low risk = .66/.67

### 2. SMOTE Oversampling

![](Resources/Capture2.PNG)

- Balanced Accuracy: 0.6303296388959394
- Precision: The precision is low for High-risk loans and is high for Low-risk loans.
- Recall: High/Low risk = .62/.64

### 3. Undersampling

![](Resources/Capture3.PNG)

- Balanced Accuracy: 0.6303296388959394
- Precision: The precision is low for High-risk loans and is high for Low-risk loans.
- Recall: High/Low risk = .63/.40

### 4. Combination Under-Over Sampling

![](Resources/Capture4.PNG)

- Balanced Accuracy: 0.5173713090878325
- Precision: The precision is low for High-risk loans and is high for Low-risk loans.
- Recall: High/Low risk = .70/.57

### 5. Balanced Random Forest Classifier

![](Resources/Capture5.PNG)

- Balanced Accuracy: 0.7877672625306695
- Precision: The precision is low for High-risk loans and is high for Low-risk loans.
- Recall: High/Low risk = .67/.91

### 6. Easy Ensemble AdaBoost Classifier

![](Resources/Capture6.PNG)

- Balanced Accuracy: 0.925427358175101
- Precision: The precision is low for High-risk loans and is high for Low-risk loans.
- Recall: High/Low risk = .91/.94

## Summary

In reviewing all six models, the EasyEnsembleClassifer model yielded the best results with an accuracy rate of 93.2% and a 9% precision rate when predicting "High Risk candidates. The sensitivity rate (aka recall) was also the highest at 92% compared to the other models. The result for predicting "Low Risk" was also the highest with the sensitivity rate at 94% and an F1 score of 97%. Therefore, if a model needed to be recommended to perform this type of analysis, then this one would be the clear choice.
