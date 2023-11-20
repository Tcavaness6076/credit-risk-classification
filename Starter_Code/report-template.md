# Module 12 Report Template

## Overview of the Analysis

In this Analysis we started with splitting the data into target variable (y) and features variable (x). We then split our data into training and scaling. We implemented a Logistic Regression model to the test portion of our model and then we used that to make predictions. We used evaluation metrics such as Balance Accuracy Score, Confusion Matrix and Classification Report to compute the models performance.

We noticed an imbalanced distribution of loans (75,000 Healthy and only 2500 high risk). To amend this we implemented a random oversampling to balance our two classes. We then applied the same Logistic Regression, created Predictions and used the same evaluation metric on the oversampled data.

## Results

Logistic Regression on Training Data:

* Balanced accuracy score: 95.20%
* Precision for healthy loans: 100%
* Recall for healthy loans: 99%
* Precision for high-risk loans: 85%
* Recall for high-risk loans: 91%

Oversampled Data Logistic Regression:

* Balanced accuracy score: 99.36%
* Precision for healthy loans: 100%
* Recall for healthy loans: 99%
* Precision for high-risk loans: 84%
* Recall for high-risk loans: 99%

## Summary

We found that the oversampled data out performed the original data. While we did maintain a consistent result of healthy loans for both models, our high risk recall was enhanced by the oversampling. We were able to achieve a 99% recall for high-risk loans in the oversampled data vs. a 91% originally. This is a crucial improvement for reducing the number of approved high-risk loans. This allows us to prioritize approving healthy loan clients over high precision for high-risk loans.
