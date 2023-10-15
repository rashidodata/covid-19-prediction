# Predicting-COVID-19-condition-and-hospitalization-levels-using-blood-analysis-and-test-results
This projects aims to predict whether the patient has been infected by COVID-19, as well as s/he is hospitalized in one of the three units: regular ward, semi intensive or intensive care unit meaning that there are four target variables to predict. The dataset is small, has high number of missing values and as expected, highly imbalanced. It contains wide range of blood test variables which will form the main features of the model and other test variables with small variation which makes them challenging to use in the model.

We first do exploratory data analysis and try to identify the key features to use in the model. We notice that blood count variables are weakly correlated with target variables. To improve the correlation, we employ feature engineering which creates dummy variables based on optimal thresholds. The details of the algorithm can be found in the code. 

We then use Logistic Regression and SVM with Grid Search for the prediction. To improve the results, we also add PCA to SVM model. Overall results are quite satisfactory (>0.70 AUC test score for all target variables) given the challanges with the data. 

Please see the code for more details. 
