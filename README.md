# Bike_Sharing_Demand_Prediction

## Problem Statement
Currently Rental bikes are introduced in many urban cities for the enhancement of mobility comfort. It is important to make the rental bike available and accessible to the public at the right time as it lessens the waiting time. Eventually, providing the city with a stable supply of rental bikes becomes a major concern. The crucial part is the prediction of bike count required at each hour for the stable supply of rental bikes. The main objective is to make predictive model, which could help them in predicting the bike demands proactively. This will help them in stable supply of bike wherever needed.

## Project Summary
A bike-sharing system provides people with a sustainable mode of transportation and has beneficial effects for both the environment and the user. In recent days, Pubic rental bike sharing is becoming popular because of is increased comfortableness and environmental sustainability. Data used include Seoul Bike and Capital Bikeshare program data. Data have weather data associated with it for each hour. For the dataset, we are using linear regression model were train with optimize hyperparameters using a repeated cross validation approach and testing set is used for evaluation. Multiple evaluation indices such as 𝑅 2 , Root Mean Square error are use to measure the prediction performance of the regression models. The performance of the model is vary with the time interval used in transforming data.

There were 8760 rows and 14 columns in our data that were consisting, Date,Rental Bike count ,Hour ,Temperature,Humidity,Windspeed,Visibility,Dew point temperature,Solar radiation,Rainfall,Snowfall,Seasons,Holiday,Functional Day.

Currently Rental bikes are introduced in many urban cities for the enhancement of mobility comfort. It is important to make the rental bike available and accessible to the public at the right time as it lessens the waiting time. Eventually, providing the city with a stable supply of rental bikes becomes a major concern. The crucial part is the prediction of bike count required at each hour for the stable supply of rental bikes. The main objective is to make predictive model, which could help them in predicting the bike demands proactively. This will help them in stable supply of bike wherever needed.

Null values are a big problem in machine learning . If you are using sklearn, or any other machine learning packages, it is required to clean up null values before you pass your data to the machine learning framework. Otherwise, it will give you a long and ugly error message. So we are checking for null/ missing values. There is no missing value and no null value in provided dataset.

Data cleaning is the foremost step in any data science project. No data is clean, but most is useful. Data cleaning is the process of detecting and correcting (or removing) corrupt or inaccurate records from a record set, table, database and refers to identifying incomplete, incorrect, inaccurate or irrelevant parts of the data and then replacing,modifying, or deleting the dirty or coarse data. To begin with our data cleaning, first we check for duplicate values and there is no duplicate values in given dataset. After doing so we are converting datatypes, and then we have done exploratory data analysis and find best fit model of dataset.

In statistics, exploratory data analysis (EDA) is an approach of analyzing data sets to summarize their main characteristics, often using statistical graphics and other data visualization methods. A statistical model can be used or not, but primarily EDA is for seeing what the data can tell us beyond the formal modeling and thereby contrasts traditional hypothesis testing. EDA is helped us figuring out various aspects and relationships among the target and the independent variables.

The target variable of the dataset is the feature of a dataset about which you want to gain a deeper understanding. In our data, the column ‘Rental Bike Count’ contains the value we need to predict i.e. the target variable is ‘Rental Bike Count’. Here is the target parameter Rental Bike Count distribution analysis plot and plot is positively skewed.for making it normally distribute we use square root transform.

The present analysis of Bike_sharing_demand_prediction using supervised regression method was quite challenging but it provided us lots of insights. As the dataset is huge, so I have use different regression models to get the better prediction.

Model performance for the Linear Regression, Lasso Regression, Ridge Regression,ElasticNet is not showing good performance for MSE, RMSE, R^2 and Adjusted R^2 value.

The model performance for the Decision Tree Rregressor, XGBoost Regressor and Random Forest Regressor finally showed some good performance for MSE, RMSE , R^2 and Adjusted R^2 value.

For R^2 and Adjusted R^2 all above mentioned regressors showed a better running model.

But among all the used models for ML regression analysis, XGBoost Regressor showed the best performance with r2= 0.923651 and Adjusted R^2=0.922184
