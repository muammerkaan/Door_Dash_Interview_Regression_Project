# Door_Dash_Interview_Regression_Project
This is a project from https://platform.stratascratch.com/data-projects/delivery-duration-prediction that aims to predict the delivery duration of orders placed on door dash.

# Feature Engineering
* Creating dependant variable.
* Creating 3 useful predictor variables.
* One hot encoding 3 categorical variables. 

# Data Preprocessing
* Drop unnecessary features.
* Concat dummy variables to our training dataset.
* Align data types across the whole dataset.
* Drop infinite values.

# Removing Collinear Features
* Create correlation matrix to look for outliers.
* Define two functions that will help us find the pairs of features with the highest correlation values.
* Feature engineer and drop redundant features to eliminate collineararity from our dataset.

# Reducing Multicollinearity
* Define a function that computes the vif score for each of the features and sorts them in order.
* Use a while loop to drop all features with a vif score greater than 20.

# Feature Selection
* Use RandomForestRegressor to find the Gini importance of all the features in the dataset.
* Use PCA to find the optimum number of features to represent our dataset.

# Scaling
* Define a function to apply different scalars to our data.

# Model Building
* Find the optimum regression model, feature size and scalar by comparing the RMSE scores.
* Feature engineer a new dependant variable to see if we can decrease the RMSE score.
* Use the predicitons of our new dependant variable as an independant variable in a new regresion model that will the predict the total_duration.

# Deep Learning
* Use Keras to apply an ANN to our data.

# Outcome
The official solution was an LGBM + Linear Regression model that had a RMSE of 986.6912510303843 
