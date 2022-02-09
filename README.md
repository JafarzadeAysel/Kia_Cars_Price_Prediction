# KIA Cars Price Prediction:  Project Overview 
* Created a tool that estimates Kia car's market price in Azerbaijan to help sellers/buyers to make the best decisions for their sale/purchase 
* Scraped over 4000 car advertisement descriptions from Turbo.az and analyzed them using Python
* Cleaned dataset and proceeded with Feature Engineering
* Tested different algorithms for given regression problem such as Linear, Lasso and Decision Tree Regressions
* Compared the Accuracy Score and Root Mean Squared Error of these models to see which model performs better

## Code and Resources Used
* Python Version: 3.7  
* Packages: pandas, numpy, BeautifulSoup, matplotlib, scipy, sklearn, pickle
* Link to Dataset: https://drive.google.com/open?id=1mrKSmWdOZnAI59jaRYEgS99zQJF8pOZg

## Web Scraping
From each car description following features were collected:
* City
* Brand
* Model
* Year
* Body Type
* Color
* Engine
* Engine Power
* Fuel Type
* Kilometrage
* Transmission
* Drivetrain
* New or not
* Price

## Data Cleaning and Feature Engineering
Applied data cleaning and feature engineering to make data better suited to the problem at hand:
* Cleaned duplicate values and fixed inconsistencies in some columns 
* Outliers detected by using standard deviation and handled
* Dimensonality reduction applied to some categorical columns for encoding 
* Transformed the categorical variables into dummy variables


## Machine Learning: Predictive Modelling
I tried three different models and evaluated them using Accuracy score and RMSE. I chose RMSE becacuse outliers already cleaned and it seemed as best option
* Split the data into train and tests sets with a test size of 20%.
* Tested different algorithms for given regression problem such as Linear, Lasso and Decision Tree Regressions
* Trial models were SVM, Random Forest, Logistic Regression
* Best performed model: SVM

## Model Performance
* The metric used for the models’ evaluation is the ROC and AUC


## Visuals
![alt text](https://github.com/JafarzadeAysel/Bank_Loan_Default_Prediction/blob/main/default_non.PNG "Defaults vs Non-Defaults in imbalanced data")
![alt text](https://github.com/JafarzadeAysel/Bank_Loan_Default_Prediction/blob/main/roc-auc.PNG "ROC - AUC curve of model")
