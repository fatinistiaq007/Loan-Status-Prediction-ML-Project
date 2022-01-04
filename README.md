# Loan-Status-Prediction-ML-Project
## Final Report
#### (1) For training data set,  the features 'Principal','terms','age','Gender','weekend' + one-hot-encoded 'education', with normalization, were obtained results: 
##### KNN works best with k=7 
##### Decision Tree works best with max_depth=15 
##### SVM works best with kernel='rbf' 
##### Logistic Regression works best with C=0.1 

#### Accuracy metrics are: 

#### |Algorithm||Jaccard||F1-score||LogLoss|
#### |   KNN   ||  0.8  ||  0.46  ||  NA   |
#### |   Decision Tree   ||  0.78  ||  0.45  ||  NA   |
#### |   SVM   ||  0.78  ||  0.15  ||  NA   |
#### |   LogisticRegression   ||  0.71  ||  0.258  || 0.50   |


#### (2) For testing data set,  the features 'Principal','terms','age','Gender','weekend' + 'education' replaced by 1 numeric column (see above), with normalization, were obtained the same best parameters: 
##### KNN works best with k=7 
##### Decision Tree works best with max_depth=15 
##### SVM works best with kernel='rbf' 
##### Logistic Regression works best with C=0.1 

#### But accuracy metrics are not the same:  

|Algorithm||Jaccard||F1-score||LogLoss|
|   KNN   ||  0.6481  ||  0.239  ||  NA   |
|   Decision Tree   ||  0.72  ||  0.44  ||  NA   |
|   SVM   ||  0.7407  ||  0.0  ||  NA   |
|   LogisticRegression   ||  0.7407  ||  0.0  || 0.4825   |

#### As we can see, KNN and LogisticRegression work better in the case (1), Decision Tree shows almost similar results in both the case (1) and (2). SVM might be considered to work better in the case (2), but F1-score=0 means that there are no predicted samples; so it is bad.
