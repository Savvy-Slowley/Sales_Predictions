# Overview

This project will be a sales prediction for food items sold at various stores. I will demostrate decision making through data cleaning, complete any statistical analyses that might help you understand, explain, or model with your data.build several data visualizations to help your stakeholders better understand trends in the data.your task is to use Linear Regression to create and evaluate a model to predict sales:

Use the data you have cleaned in previous weeks. 
Spend time transforming your categorical variables into numbers and use dummy encoding where appropriate.
Here are some resources to use when dealing with categorical variables:
Dealing with categorical features in machine learning
Categorical Data
Here’s All you Need to Know About Encoding Categorical Data (with Python code)
Assign the "Item_Outlet_Sales" column as your target and the rest of the variables as your features matrix.  
Be sure to train test split your data set!
Build a linear regression model.
Evaluate your test set results using r2.
Evaluate your test set results using RMSE
Which features are most associated with higher predicted sales?
Your task is to build tree based models to predict sales and compare evaluation metrics for regression problems.  

Build and evaluate a simple decision tree model.
Build and evaluate a bagged tree model.
Build and evaluate a random forest model.  
You now have tried at least 4 models on this data set (including the regression model from last week).  Compare the performance of your models based on r^2.
Compare the performance of your models based on rmse.  
Overall, which model do you recommend?


# Data Dictionary

Here is the Data Dictionary for this dataset:

Variable Name	Description:

Item_Identifier	- Unique product ID

Item_Weight - Weight of the product

Item_Fat_Content - Whether the product is low fat or regular

Item_Visibility - The percentage of the total display area of all products in a store allocated to the particular product

Item_Type - The category to which the product belongs

Item_MRP - Maximum Retail Price (list price) of the product

Outlet_Identifier - Unique store ID

Outlet_Establishment_Year - The year in which the store was established

Outlet_Size - The size of the store in terms of ground area covered

Outlet_Location_Type - The type of area in which the store is located

Outlet_Type - Whether the outlet is a grocery store or some sort of supermarket

Item_Outlet_Sales - Sales of the product in the particular store. This is the target variable to be predicted.
