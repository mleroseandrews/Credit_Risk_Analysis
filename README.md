# Credit_Risk_Analysis

## Overview of the analysis: 
This project was designed to use machine learning to look at credit card risk.  The low class risk outnumbers the high class  risk.   We use different resampling techniques to resolve the class imbalance.  

## Results

- Naive Random Oversampling -         Balanced Accuracy 66%, High-risk Precision .01, High-risk Recall .69, High-risk F1 Score .02
- SMOTE Oversampling -                Balanced Accuracy 66%, High-risk Precision .01, High-risk Recall .63, High-risk F1 Score .02
- Cluster Centroids Undersampling -   Balanced Accuracy 66%, High-risk Precision .01, High-risk Recall .63, High-risk F1 Score .02
- SMOTEENN -                          Balanced Accuracy 64%, High-risk Precision .01, High-risk Recall .71, High-risk F1 Score .02
- Balanced Random Forest Classifier - Balanced Accuracy 78%, High-risk Precision .03, High-risk Recall .70, High-risk F1 Score .06
- Easy Ensemble AdaBoost -            Balanced Accuracy 93%, High-risk Precision .09, High-risk Recall .92, High-risk F1 Score .16

## Summary

Of the six resampling techniques and models, the SMOTEENN technique was the lowest performing. With an accuracy score of 0.64 and a high-risk precision of 0.01. The best performing model was the EasyEnsembleClassifier. This model obtained a high accuracy score of 0.93, and predicted high risk credit at a much higher rate than the other five techniques (0.09).  Out of the 101 high risk loan applications in the test data, this model correctly identified 93 and incorrectly classified 8 of them as low-risk. Based on the accuracy level, I would reccommend the Easy Ensemble AdaBoost Classifier.
