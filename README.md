# Bank Loan Default Prediction:  Project Overview 
* Built a tool to understand the past customers' profile in order to minimize the risk of future loan defaults
* Cleaned dataset and use Future Selection Method
* Tried models like SVM, Random Forest, Logistic Regression and chose best one using K-Fold Cross-Validation
* Used GridsearchCV for Hyper Parameter Tuning
* Visualized ROC - AUC curve to evaluate the performance of model

## Code and Resources Used
* Python Version: 3.7  
* Packages: pandas, numpy, sklearn, matplotlib
* Link to Dataset: https://drive.google.com/open?id=1mrKSmWdOZnAI59jaRYEgS99zQJF8pOZg

## Project structure
The project divides into two categories:
* Data Wrangling: Cleansing and Feature Selection
* Machine Learning: Predictive Modelling

## Data Wrangling: Cleansing and Feature Selection
There was need to clean dataset so that it was useable for our model. I made the following changes and created the following variables:
* Added a column for if the loan was in default
* Checked if data is imbalanced and found a way to handle this problem
* Removed columns those had highest percentage of missing values
* Investigated cardinality and dropped zero variance columns
* Imputed missing values of different types of colummns by building pipelines for each
* Selected best 20 features of dataset with SelectKBest


## Machine Learning: Predictive Modelling
* Split the data into train and tests sets with a test size of 20%.
* Tried three different models and chose one of them using K-Fold Cross-Validation
* Trial models were SVM, Random Forest, Logistic Regression
* Best performed model: SVM

## Model Performance
* The metric used for the models’ evaluation is the ROC and AUC


## Visuals
![alt text](https://github.com/JafarzadeAysel/Bank_Loan_Default_Prediction/blob/main/default_non.PNG "Defaults vs Non-Defaults in imbalanced data")
![alt text](https://github.com/JafarzadeAysel/Bank_Loan_Default_Prediction/blob/main/roc-auc.PNG "ROC - AUC curve of model")
