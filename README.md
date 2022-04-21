# Assignment

The objective of the given problem was to solve the binary classification problem using the classical ML algorithm. I have trained various model for the binary classification problem. There were total of 3910 data point was given for the training having 56 different numerical features. 

## EDA 

Key Observation from the EDA
1. Few columns has very sparsed data. More than 70-80% rows has no values. i.e Column X4, X1, X7, X31
2. While few columns have a fair distribution of non-zero values but those are very skewed distribution i.e X56, X57 columns
3. Also different data columns are on different sacles like columns X51 is between 0 to 2.78 while X57 is between 1 to ~10k

## Preprocessing + Feature Selection 

I have used the followoing two methods to check the sanity of each feature and the feature importance. 
1. Variance Thresholding
2. Matual Information 

Note: No data points were missing Hence no imputation required here. 

## Modeling

I have tried following classification models. 

1. Random Forest
2. XGBoost
3. SVM

## Evaluation

Here are the result of the best prformed model. 

1. Training Accuracy :  0.99808
2. Testing Accuracy :  0.96036
3. AUC-ROC Score : 0.98947
4. Classification Report:  


              precision    recall  f1-score   support

           0       0.97      0.96      0.97       478
           1       0.94      0.96      0.95       304

    accuracy                           0.96       782
   macro avg       0.96      0.96      0.96       782
weighted avg       0.96      0.96      0.96       782

