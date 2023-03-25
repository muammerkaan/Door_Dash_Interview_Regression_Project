# DoorDash Interview Regression Project
This is a project from https://platform.stratascratch.com/data-projects/delivery-duration-prediction that aims to predict the delivery duration of orders placed on door dash.

### Data Preperation
* Feature engineering is preformed in order to produce useful predictor variables for our model as well as reduce collinearity. 
* Drop redundant features that cause collinearity in the data.
* Drop features that have high VIF scores as they will cause multicollinearity in the data.
* Use RandomForestRegressor to find the Gini importance of all the features in the dataset.
* Use PCA to find the optimum number of features to represent our dataset.

### Model Building
* Apply Apply 6 different regression algorithims (Ridge Regression, Decision Tree Regressor, Random Forrest Regressor, XGBoost Regressor, LGBM Regressor, MLP Regressor), 4 different feature set sizes selected by Gini importance and 3 different scalars (Standard Scalar, Min-Max Scalar, No scalar).
* Find the optimum combination of algorithim, feature set size and scalar by comparing the RMSEs.
* Feature engineer a new dependant variable to try and reduce the RMSE.
* Use the predicitons of our new dependant variable as an independant variable in a new regresion model that will the predict the total_duration.
* Apply an ANN using keras and compare results with our classical machine learning models.

### Outcome
The official solution was an LGBM + Linear Regression model that had a RMSE of 986.6912510303843 
