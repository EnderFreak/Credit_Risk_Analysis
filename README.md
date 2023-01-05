# Credit_Risk_Analysis

## Overview of the analysis
Using credit card dataset from LendingClub, a peer-to-peer lending services company, I have to use my skills in data preparation, statistical reasoning and machine learning to assess credit card risk.  
Using different Machine Learning models of samplings to reduce bias, I was tasked by Jill to evaluate the performance of these models and whether they should be used to predict risk.

## Results
#### USING RANDOMOVERSAMPLER ALGORITHM
![RandomOverSampler](images/randomoversampler.png)

* Accuracy score is about 63%
* Precision is very low for high-risk loan statuses, but very accurate for low-risk
* Sensitivity/Recall is high for low-risk loan status, but low for high-risk class
* We note a pronounced imbalance between sensitivity and precision for the high-risk loan_status people - making the F1 score very low (0.02)

#### USING SMOTE ALGORITHM
![SMOTE](images/smote.png)

* Accuracy score is about 63%
* Precision is very low for high-risk loan statuses, but very accurate for low-risk
* Sensitivity/Recall is high for both low and high-risk loan statuses

#### USING CLUSTER CENTROIDS ALGORITHM
![Cluster Centroids](images/clustercentroids.png)

* Accuracy score is about 53%
* Precision is very low for high-risk loan statuses, but very accurate for low-risk
* Sensitivity/Recall is low for low-risk loan status, and high for high-risk class

#### USING SMOTEENN ALGORITHM
![SMOTEENN](images/smoteenn.png)

* Accuracy score is about 64%
* Precision is very low for high-risk loan statuses, but very accurate for low-risk
* Sensitivity/Recall is high for both low and high-risk loan statuses

#### USING BALANCED RANDOM FOREST CLASSIFIER
![Balanced Random Forest Classifier](images/balancedrandomforestclassifier.png)

* Accuracy score is about 79%
* Precision is very low for high-risk loan statuses, but very accurate for low-risk
* Sensitivity/Recall is high for both low and high-risk loan statuses

#### USING EASY ENSEMBLE ADABOOST CLASSIFIER
![Easy Ensemble Adaboost Classifier](images/adaboostclassifier.png)

* Accuracy score is about 93%
* Precision is very low for high-risk loan statuses, but very accurate for low-risk
* Sensitivity/Recall is very high for both low and high-risk loan statuses

## Summary
All of the Machine Learning models used to sample the data to assess credit risk result in a low and weak precision. The AdaBoost model or EasyEnsembleClassifier model was a better algorithm compared the other ones used, with an accuracy score of 93%, yet even if the precision to determine if lending a loan is high risk was very low (7% only), it is the ML model I would advise Jill to use to predit credit risk.
