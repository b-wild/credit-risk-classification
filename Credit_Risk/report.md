## Overview of the Analysis

The analysis uses a dataset of historical lending activity from a peer-to-peer lending services company to build a model that can identify the creditworthiness of borrowers. 

* The model is design to predict the creditworthiness of borrowers by using the "loan status" feature of the dataset.
* The stages of the machine learning process include creating the X and Y elements, seperate the training and test data, standardized the data through Standardscaler, trained the model, and then resampled the data.
* The methods used were a `LogisticRegression` model and a resampling method.

## Results

The balanced accuracy scores and the precision and recall scores of 'LogisticRegression' machine learning models.

* Machine Learning Model 'LogisticRegression':
  * Confusion Matrix
Predicted 0	Predicted 1
Actual 0	18652	113
Actual 1	10	609
Accuracy Score : 0.9936545604622369
Classification Report
              precision    recall  f1-score   support

           0       1.00      0.99      1.00     18765
           1       0.84      0.98      0.91       619

    accuracy                           0.99     19384
   macro avg       0.92      0.99      0.95     19384
weighted avg       0.99      0.99      0.99     19384



* Machine Learning Model 'Resampling':
  * Confusion Matrix
Predicted 0	Predicted 1
Actual 0	18652	113
Actual 1	10	609
Accuracy Score : 0.9938093272802311
Classification Report
              precision    recall  f1-score   support

           0       1.00      0.99      1.00     18765
           1       0.84      0.99      0.91       619

    accuracy                           0.99     19384
   macro avg       0.92      0.99      0.95     19384
weighted avg       0.99      0.99      0.99     19384

## Summary

Summary the results of the machine learning models, and recommendation the 'LogisticRegression' model to use:
* The logistic regression model was able to prodict both healthy and high-risk loans with a 99 - 100% accuracy, as well has having a weighted average presision and recale of 99%.  
* The precision and f1-score for the high-risk loans are lower then those of the healthy loans, however that could be due to the lower sample size as the weighted average is 99%.
* The resampled data provided nearly identical results as the original sample.  
* There was a slight decrease inthe precision for the high-risk loans which remain a mush smaller sample size compared to the healthy loans.


