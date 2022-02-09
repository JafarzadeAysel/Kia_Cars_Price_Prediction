# Kia Cars Price Prediction:  Project Overview 
* Created a tool that estimates market price of Kia cars in Azerbaijan to help sellers/buyers to make the best decisions for their sale/purchase 
* Scraped over 3000 car advertisement descriptions from Turbo.az using Python
* Cleaned dataset, analyzed patterns and proceeded with Feature Engineering
* Tested different algorithms for given regression problem such as Linear, Lasso and Decision Tree Regressions
* Compared the Accuracy Score and Root Mean Squared Error of these models to see which model performs better

## Code and Resources Used
* Python Version: 3.7  
* Packages: pandas, numpy, BeautifulSoup, matplotlib, plotly, scipy, sklearn, pickle

## Web Scraping
Following features were collected from each car description:
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
* Dimensionality reduction applied to some categorical columns for transformation in the dummy variables
* Converted the categorical variables into dummy variables

## EDA
I tried to deliver meaningful insights from the data for a car buyer in Azerbaijan
<img src="https://github.com/JafarzadeAysel/Kia_Cars_Price_Prediction/blob/4d0a359c634463b1d30181b3f5bc3f97d60e4395/by_regions.PNG" width="450" height="350">
![alt text](https://github.com/JafarzadeAysel/Kia_Cars_Price_Prediction/blob/4d0a359c634463b1d30181b3f5bc3f97d60e4395/by_regions.PNG "Cars by regions")
![alt text](https://github.com/JafarzadeAysel/Kia_Cars_Price_Prediction/blob/7f89a09b05ac93660046ccf70dec549a40d1ee66/expensive_cars.PNG "Most Expensive cars")
![alt text](https://github.com/JafarzadeAysel/Kia_Cars_Price_Prediction/blob/9f4217d753459cf659280b7d42d946bfdc20d6e3/price_distribution_cars.png "Price distribution of cars")

## Model Building
I've tried three different models and evaluated them using Accuracy score and RMSE. I chose RMSE becacuse outliers already cleaned and it seemed as best option for evaluation
* Split the data into train and tests sets with a test size of 20%.
* Tested different algorithms such as Multiple Linear, Lasso and Decision Tree Regressions
* Compared the Accuracy Score and Root Mean Squared Error of these models to see which model performs better

## Model Performance
* Multiple Linear Regression model outperformed others  
![alt text](https://github.com/JafarzadeAysel/Kia_Cars_Price_Prediction/blob/ddccff5daf8d9d325211fc9fc22f3fce2dfb047b/comparison.PNG "Models comparison")
