# project6_Patient_Survival_Prediction

## Business Problem: 
The predictors of in-hospital mortality for admitted patients remain poorly characterized. It is important to develop and validate a prediction model for all-cause in-hospital mortality among admitted patients, and identify factors that are most relevant to the ICU survival rate. The goal of this project is to provide clinical research and public health professionals with valuable insights, save lives by increasing patients’ survival rates, and ultimately bring a positive impact to the community. 

## Data Processing:
Impute numeric missing values with interpolation. Replace categorical missing values with the most frequent categories in columns. 

## EDA
Compute a series of plots, including pie charts, bar charts, line charts, and correlation matrix plot. Generate useful insights from data. 

## Feature engineering:
Encode categorical variables. Utilize SMOTE resampling method to resolve the issue of imbalanced response variable, hospital_death. Apply principal component analysis (PCA) for demision reduction. 

## Models Construction:
Apply decision tree random forest, logistic regression, and K-NN to training dataset. Plot confusion matrix and ROC curves. Since the random forest model has the highest cv accuracy, I use this model to predict patient survival rate. None of the models have overfitting issue, as cv accuracies and test accuracies are roughly equal. 
