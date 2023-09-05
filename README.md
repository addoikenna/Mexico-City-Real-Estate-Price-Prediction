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

## Predicting Apartment Prices with Neighborhood 
This **predict_price_with_neighborhood** notebook builds a model to predict apartment prices in Mexico City based on the neighborhood (borough).

#### **Data**
The data comes from a CSV file with the following features:
1. borough - the neighborhood or borough in Mexico City
2. price_aprox_usd - the apartment price in USD
#
### **Approach**
The steps taken in the notebook are:

1. Import and explore the data
2. Split into training feature and target
3. Create a baseline prediction using the mean price
4. One-hot encode the categorical borough feature
5. Build a linear regression model pipeline
6. Evaluate on the training data
7. Predict on the test data
8. Extract model coefficients and feature importances
9. Switch to Ridge regression to reduce overfitting
10. Extract Ridge model coefficients and feature importances
11. Visualize Ridge feature importances

#### **Key Findings**
1. The linear model reduces the training MAE to around $15,000
2. Ridge regularization further reduces overfitting
3. The most important features are boroughs like San Ángel, Del Valle Centro, Escandón, etc.

#### **Future Work**
Some ways the model could be improved:
1. Add more features like size, bedrooms, other amenities
2. Try different regularization techniques
3. Ensemble methods like random forests could help too.
4. Broaden data to more Mexican cities.
