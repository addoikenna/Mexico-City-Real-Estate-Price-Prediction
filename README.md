# Mexico-City-Real-Estate-Price-Prediction
This repository contains a Jupyter notebook that predicts the price of apartments in Mexico City based on their size, location (longitude and latitude) and neighborhood. The notebook uses a linear regression and ridge model. 

## Predicting Apartment Price with Size
The **predict_price_with_size** notebook first explores the relationship between apartment prices and size using descriptive statistics and visualizations. It then splits the data into a training set and a test set. The linear regression model is trained on the training set and evaluated on the test set.

The results show that the linear regression model can predict apartment prices with a mean absolute error of $1100 USD. The model also shows that larger apartments tend to have higher prices.

The notebook also includes a section on communicating the results of the analysis. This section includes the model equation, the model intercept and coefficient, and a visualization of the model.

## Predicting Apartment Price with Location (Longitude and Latitude)
The **predict_price_with_location** notebook contains code and analysis for predicting apartment prices in Mexico City using location data.

1. Price of apartment in USD
2. Location: Latitude and longitude coordinates
#### **Analysis**
The following analyses are included in the notebook:
1. Exploratory data analysis through data visualization
2. Training a baseline mean price model
3. Building a regression pipeline with imputation and model
4. Evaluating model performance on training and test sets
#### **Model**
A linear regression pipeline is implemented with the following steps:
1. Impute missing values using mean imputation
2. Fit a linear regression model to predict price based on latitude and longitude
#### **Results**
The location features are found to not be strong predictors of apartment price.
The model has similar performance to just predicting mean price
