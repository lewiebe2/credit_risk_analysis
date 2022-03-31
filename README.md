# **Credit Risk Analysis**

## **Overview**

The purpose of this analysis is to predict credit risk for client LendingClub, a peer-to-peer lending services company, by using the imbalanced-learn and scikit-learn libraries to build and evaluate resampling and ensemble classifiers models.

## **Results**

Six machine learning models were built using the LoanStats_2019Q1.csv dataset. The results have been grouped below by resampling or ensemble classifier.

### **Resampling Models Results:**

#### *1) Naive Random Oversampling*
  
  The balanced accuracy score was 0.6463970560994359 with precision scores of 0.01 for high risk and 1.00 for low risk, and recall scores of 0.71 for high risk and       0.58 for low risk.
  
  ![](Results_Images/RandomOversampler_results.PNG)

#### *2) SMOTE Oversampling*
  
  The balanced accuracy score was 0.6586230769943224 with precision scores of 0.01 for high risk and 1.00 for low risk, and recall scores of 0.63 for high risk and       0.68 for low risk.
  
  ![](Results_Images/SMOTE_bal_acc_score.PNG)
  ![](Results_Images/SMOTE_class_report.PNG)
  
#### *3) Cluster Centroids Undersampling*
  
  The balanced accuracy score was 0.5447339051023905 with precision scores of 0.01 for high risk and 1.00 for low risk, and recall scores of 0.69 for high risk and       0.40 for low risk.
  
  ![](Results_Images/ClusterCentroids_results.PNG)
  
#### *4) SMOTEENN Combination (Over and Under) Sampling*

  The balanced accuracy score was 0.6664711051320287 with precision scores of 0.01 for high risk and 1.00 for low risk, and recall scores of 0.73 for high risk and       0.60 for low risk.
  
  ![](Results_Images/SMOTEENN_results.PNG)
  
   
### **Ensemble Classifiers Results:**

#### *5) Balanced Random Forest Classifier*
 
  The balanced accuracy score was 0.7885466545953005 with precision scores of 0.03 for high risk and 1.00 for low risk, and recall scores of 0.70 for high risk and       0.87 for low risk.
  
  ![](Results_Images/BalancedRandomForestClassifier_results.PNG)

#### *6) Easy Ensemble AdaBoost Classifier*
 
  The balanced accuracy score was 0.9316600714093861 with precision scores of 0.09 for high risk and 1.00 for low risk, and recall scores of 0.92 for high risk and       0.94 for low risk.
  
  ![](Results_Images/EasyEnsembleClassifier_results.PNG)

## **Summary** 

The resampling models may not be the best for predicting credit risk because the models' balanced accuracy scores are all less than 0.70 which is low, and the precision and recall scores are not good enough to state that the model will be good at classifying high credit risk. 

The ensemble classifier models performed much better with balanced accuracy scores greater than 0.75, better precision scores, and strong recall scores over 0.70. The easy ensemble AdaBoost classifier model is a very strong predictor of high credit risk with all scores greater than 0.90. Of the six models, the easy ensemble AdaBoost classifier model should be used.
