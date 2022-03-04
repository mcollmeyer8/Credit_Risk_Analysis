# Credit_Risk_Analysis

## Overview of the Analysis
Using several different machine learning techniques, I analyzed credit card data to predict credit risk.

## Results
Using an unbalanced data set that included 68,470 low risk individuals and 347 high risk individuals, I used several sampling techniques to analyze the data and predict credit risk.

### Naive Random Oversampling
- First, I used RandomOversampler from the imblearn library to resampled the data. Results are as follows:
- Balanced accuracy score of 0.6413 or 64.13%
- Precision score (% of positive predictions that are correct): 0.00955 or 0.955%
- Recall score (% of actual positive results that are predicted correctly): 0.5977 or 59.77%

### SMOTE Oversampling
- Next, I used SMOTE (Synthetic Minority Oversampling) also from the imblearn library to resample the data. Results are as follows:
- Balanced accuracy score of 0.6374 or 63.74%
- Precision score: 0.0093 or 0.93%
- Recall score: 0.5977 or 59.77%

### Undersampling
- Next, I undersampled the data using the Cluster Centroids algorithm.
- Balanced accuracy score of 0.5292 or 52.92%
- Precision score: 0.0055 or 0.55%
- Recall score: 0.6092 or 60.92%

### Combination (Over and Under) Sampling
- For this activity, I resampled the data using the SMOTEENN algorithm.
- Balanced accuracy score of 0.6376 or 63.76%
- Precision score: 0.0083 or 0.83%
- Recall score: 0.7011 or 70.11%

### Balanced Random Forest Classifier
- I next resampled the data using the ensemble algorithm BalancedRandomForestClassifier.
- Balanced accuracy score of 0.8104 or 81.04%
- Precision score (% of positive predictions that are correct): 0.0344 or 3.44%
- Recall score (% of actual positive results that are predicted correctly): 0.7241 or 72.41%

### Easy Ensemble AdaBoost Classifier
- Lastly, I used the ensemble algorithm EasyEnsembleClassifier to resample the data.
- Balanced accuracy score of 0.9254 or 92.54%
- Precision score: 0.0747 or 7.47%
- Recall score: 0.9080 or 90.8%

## Summary
The Oversampling, Undersampling and Combo models resulted in fairly similar numbers. Of these models, the Combo sampling resulted in the best numbers (balanced accuracy: 63.76%, precision score: .83% and recall score: 70.11%). That being said the ensemble algorithms generated even better numbers. If I were to recommend an algorithm to use for this project, I would recommend using the Easy Ensemble AdaBoost Classifier. The balanced accuracy score was 92.54%, with a precision score of 7.47% and recall score of 90.8%.
