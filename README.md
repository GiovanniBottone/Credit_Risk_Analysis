# Credit_Risk_Analysis

## Overview

Using a credit card credit dataset from fictional company 'LendingClub lending services,' this analysis will use multiple algorithms and methods to determine which method provides applicable results. LendingClub has specified that we:
* Oversampling the data using the RandomOverSampler and SMOTE algorithms
* Undersample the data using the ClusterCentroids algorithm
* Over and undersampling using the SMOTEENN algorithm
* Compare two new machine learning models - BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk
* Evaluate the performance of these models and provide a recommendation on whether they should be used to predict credit risk.

## Results

Naive Random Oversampling:
![Naive Random Oversampling](https://user-images.githubusercontent.com/95371617/167272662-a777dfdd-8fdc-4b48-8160-e1c6b8aa956b.png)

* The balanced accuracy score indicates that 66% of the Naive Random Oversampling model's predictions were correct.
* High risk loans have a precision of 1%, which means that of all samples pre-determined as high risk, 1% were actually high risk. Additionally, high risk loans had a recall of 72%, which means the model accurately identified 72% of all high risk loans.
* Low risk loans had a precision of 100%, with a recall of 60%, meaning that 40% of low risk loans were falsely identified as high risk. 


Smote Oversampling:
![Smote](https://user-images.githubusercontent.com/95371617/167273029-584ec95e-6fa5-425d-ac0f-46044bbaeb7e.png)

* The balanced accuracy score indicates that 63.4% of the SMOTE model's predictions were correct.
* High risk loans have a precision of 1%, which means that of all samples pre-determined as high risk, 1% were actually high risk. Additionally, high risk loans had a recall of 58%, which means the model accruately identified 58% of all high risk loans.
* Low risk loans have a precision of 100%, with a recall of 68%, meaning that 32% of low risk loans were falsely identified as high risk.


Undersampling:
![Undersampling](https://user-images.githubusercontent.com/95371617/167273177-7af733d2-90d9-47c2-8e51-fb05c79a85ab.png)

* The balanced accuracy score indicated that 54.4% ot the Undersampling model's predictions were correct.
* High risk loans have a precision of 1%, which means that of all samples pre-determined as high risk, 1% were actually high risk. Additionally, high risk loans had a recall of 69%, which means the model accurately identified 69% of all high risk loans.
* Low risk loans had a precision of 100%, with a recall of 40%, meaning that 60% of low risk loans were falsely identified as high risk. 


Overampling & Undersampling:
![Over and Under Sampling](https://user-images.githubusercontent.com/95371617/167273336-7029c6d3-4836-460f-9097-b6e68ab650d5.png)

* The balanced accuracy score indicated that 64.6% of the Oversampling & Undersampling model's predictions were correct.
* High risk loans have a precision of 1%, which means that of all samples pre-determined as high risk, 1% were actually high risk. Additionally, high risk loans had a recall of 72%, which means the model accurately identified 72% of all high risk loans.
* Low risk loans had a precision of 100%, with a recall of 57%, meaning that 43% of low risk loans were falsely identified as high risk. 


Balanced Random Forest Classifier:
![Balanced Random Forest Classifier](https://user-images.githubusercontent.com/95371617/167273402-547cc6e4-4d76-4ddb-963b-0635773563bc.png)

* The balanced accuracy score indicated that 78.9% of the Balanced Random Forest Classifier model's predictions were correct.
* High risk loans had a precision of 3%, which means that of all samples pre-determined as high risk, 3% were actually high risk. Additionally, high risk loans had a recall of 70%, which means the model accurately identified 70% of all high risk loans.
* Low risk loans had a precision of 100%, with a recall of 87%m which means that 13% of low risk loans were falsely identified as high risk.


Easy Ensemble AdaBoost Classifier:
![Easy Ensemble AdaBoost Classifier](https://user-images.githubusercontent.com/95371617/167273550-b0db2caa-988b-4256-8b1c-b9e4ae4b32eb.png)

* The balanced accuracy score indicated that 93.1% of the Easy Ensemble AdaBoost Classifier model's predictions were correct.
* High risk loans had a precision of 9%, which means that of all samples pre-determined as high risk, 9% were actually high risk. Additionally, high risk loans had a recall of 92%, which means the model accurately identified 92% of all high risk loans.
* Low risk loans had a precision of 100%, with a recall of 94% which means that 6% of low risk loans were falsely identified as high risk.

## Summary
After reviewing the models, the Easy Ensemble AdaBoost Classifier model is my recommendation due to the simple fact that it provided the highest recall rates and the highest high risk precision. With a recall rate for high risk loans of 92%, the Easy Ensemble model has the highest high risk recall rate by 20%. Also, with a high risk loans precision score of 9%, the Easy Ensemble model has the highest pre-determined to legitimaetly high risk conversion rate. This is especially important with high risk loans, because this model gives LendingClub the largest chance of identifying a high risk loan.

