# Module 12 Report Template

## Overview of the Analysis

In this analysis, the purpose was to assess the credit risk associated with loans using machine learning models. The data provided historical lending activity from a peer-to-peer lending services company, and the goal was to build models that could identify the creditworthiness of borrowers. The analysis involved predicting loan status, with a value of 0 indicating a healthy loan and 1 indicating a high risk of default.

The key stages of the machine learning process included data preprocessing, splitting the data into training and testing sets, and building logistic regression models. Two models were evaluated: one with the original data and another with resampled data using the RandomOverSampler method.

## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
  * **Balanced Accuracy Score:** 0.9520
  * **Confusion Matrix:**

   ```
   0  18663 102
   1     56 563 
   ```

  * **Classification Report:**

  ```
          precision    recall  f1-score   support
      0       1.00      0.99      1.00     18765
      1       0.85      0.91      0.88       619
  ```

* Machine Learning Model 2:
  * **Balanced Accuracy Score:** 0.9937
  * **Confusion Matrix (Resampled):**

  ```
   0  18649 116
   1      4 615
  ```

  * **Classification Report (Resampled):**

  ```
          precision    recall  f1-score   support
      0       1.00      0.99      1.00     18765
      1       0.84      0.99      0.91       619
  ```

## Summary

The resampled model (Model 2) outperforms the original model in terms of balanced accuracy, precision, and recall scores. The resampled model, designed to address imbalanced data, demonstrates superior performance in correctly identifying high-risk loans (label 1), as indicated by the higher recall score (0.99). This is crucial for a credit risk analysis, where correctly identifying high-risk loans is of utmost importance.

Considering the higher performance metrics, especially for the critical task of identifying high-risk loans, it is recommended to use the resampled model (Model 2) for credit risk analysis in this scenario.
