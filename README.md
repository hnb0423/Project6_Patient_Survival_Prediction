# Project6: Patient Survival Prediction

## Business Problem: 
The predictors of in-hospital mortality for admitted patients remain poorly characterized. It is important to develop and validate a prediction model for all-cause in-hospital mortality among admitted patients, and identify factors that are most relevant to the ICU survival rate. The goal of this project is to provide clinical research and public health professionals with valuable insights, save lives by increasing patients’ survival rates, and ultimately bring a positive impact to the community. 

## Raw Data
Link: https://www.kaggle.com/mitishaagarwal/patient

## Data Processing:
Impute numeric missing values with interpolation. Replace categorical missing values with the most frequent categories in columns. 

## EDA
Compute a series of plots, including pie charts, bar charts, line charts, and correlation matrix plot. Generate useful insights from data. 

## Feature engineering:
Encode categorical variables. Utilize SMOTE resampling method to resolve the issue of imbalanced response variable, hospital_death. Apply principal component analysis (PCA) for demision reduction. 

## Models Construction:
Apply decision tree random forest, logistic regression, and K-NN to training dataset. Plot confusion matrix and precision, recall curves. Since the random forest model has the highest cv accuracy, traning accuracy, and f1 score, I use this model to predict patient survival rate. None of the models have overfitting issue, as cv accuracies and training accuracies are roughly equal. 
