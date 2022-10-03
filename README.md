# Credit_Risk_Analysis

## Overview of the analysis:
This analysis looks at credit card risk. To accomplish this, the following libraries are going to be used to train and evaluate models: imbalanced-learn & scikit-learn. 

### Algorithms 
* RandomOverSampler 
* SMOTE
* ClusterCentroids
* SMOTEENN
* BalancedRandomForestClassifier
* EasyEnsembleClassifier

## Results:

1. BalancedRandomForestClassifier 

![RandomOverSampler ](https://user-images.githubusercontent.com/104809098/193482894-e08257cd-9dcb-4f4e-9d2a-dca86b94b487.png)

* Balance Accuracy Score - Overall model accurately predicts low and high risk categories 78% of instances.
* Precision scores - high risk precision 0.03; low risk precision 1.00.
* Recall Scores - high risk 0.70; low risk 0.87


2. EasyEnsembleClassifier

![SMOTE](https://user-images.githubusercontent.com/104809098/193482960-0c0188f5-e200-4a50-a2c1-365791053e83.png)

* Balance Accuracy Score - Overall model accurately predicts low and high risk categories 93% of instances.
* Precision scores - high risk precision 0.09; low risk precision 1.00.
* Recall Scores - high risk 0.92; low risk 0.94

3. ClusterCentroids

![ClusterCentroids](https://user-images.githubusercontent.com/104809098/193484162-a1a183cb-e373-4447-bcc8-ac42d93e2a83.png)

* Balance Accuracy Score - Overall model accurately predicts low and high risk categories 52% of instances.
* Precision scores - high risk precision 0.01; low risk precision 1.00.
* Recall Scores - high risk 0.69; low risk 0.40

4. SMOTEENN

![SMOTEENN](https://user-images.githubusercontent.com/104809098/193484470-6c76689c-aa92-4148-be21-3261b0ae4094.png)

* Balance Accuracy Score - Overall model accurately predicts low and high risk categories 64% of instances.
* Precision scores - high risk precision 0.01; low risk precision 1.00.
* Recall Scores - high risk 0.70; low risk 0.58.

5. RandomOverSampler

![BalancedRandomForestClassifierv](https://user-images.githubusercontent.com/104809098/193484878-2dd3545b-487d-4799-87fe-3b1f30f3bfa6.png)

* Balance Accuracy Score - Overall model accurately predicts low and high risk categories 64% of instances.
* Precision scores - high risk precision 0.01; low risk precision 1.00.
* Recall Scores - high risk 0.70; low risk 0.59.

6. SMOTE 

![SMOTE1](https://user-images.githubusercontent.com/104809098/193485119-e49163ec-5066-490d-ab2e-91d33d4d869e.png)

* Balance Accuracy Score - Overall model accurately predicts low and high risk categories 66% of instances.
* Precision Scores - high risk precision 0.01; low risk precision 1.00.
* Recall Scores - high risk 0.63; low risk 0.69.

## Summary:
Of all of the models tested the Easy Ensemble AdaBoost Classifier performed the strongest. This model has a high accuracy of 93%, a high precision for Low Risk and a higher precision for high risk than all other models used. Due to the low overall sample number for high risk groups it would be unrealistic to require a high precision for high risk on the testing data. The low risk recall of 94% indicates that only 6% of the testing data was misclassified for the low risk group. The application of Easy Ensemble AdaBoost Classifier on this data set appears to reasonably predict high and low risk loans. Based on the recalls, this method appears to honor both categories and as a predictive tool appears to be up for the task.

