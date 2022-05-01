# Credit Risk Analysis 
A comparison study of various machines learning models to predict credit risk

## Overview

Using LendingCLub's credit dataset, we oversampled the data using:
- RandomOversampler 
- SMOTE 

We then undersampled the data using ClusterCentroids algorithm. 

Finally, we used the combinatorial approach of SMOTEENN to sample the dataset. 

After using various sampling methods, we then employed two machine learning models to reduce bias: 
- BalancedRandomForestClassifier
- EasyEnsembleClassifier 

## Results 

### Naive Random Oversampling 
![naive](resources/naive.JPG)
1. Balanced Accuracy: .65
2. Precision: High for Low Risk, Low for High Risk 
3. Recall (High/Low): .69/.62  

### SMOTE
![naive](resources/smote.JPG)
1. Balanced Accuracy: .66
2. Precision: High for Low Risk, Low for High Risk 
3. Recall (High/Low): .63/.69

### ClusterCentroids
![naive](resources/cc.JPG)
1. Balanced Accuracy: .54
2. Precision: High for Low Risk, Low for High Risk 
3. Recall (High/Low): .40/.69

### SMOTEENN
![naive](resources/smoteenn.JPG)
1. Balanced Accuracy: .65
2. Precision: High for Low Risk, Low for High Risk 
3. Recall (High/Low): 

### BalancedRandomForestClassifier
![naive](resources/balanced_rf.JPG)
1. Balanced Accuracy: .79
2. Precision: High for Low Risk, Low for High Risk 
3. Recall (High/Low): .70/.87

### EasyEnsembleClassifier
![naive](resources/ee.JPG)

1. Balanced Accuracy: .93
2. Precision:2. Precision: High for Low Risk, Low for High Risk 
3. Recall (High/Low): .92/.94

## Summary

Of the models tested, the Easy Ensemble Classifier had the greatest accuracy with .93. The precision among the models were all very similar in that their precision scores for high_risk were extremely low. The Easy Ensemble Classifier had the highest score of .09. Recall for all low_risk were all at 1.0. 

Given the high accuracy, precision (with exception to high_risk), and recall, I would recommend using the Easy Ensemble Classifier. 

