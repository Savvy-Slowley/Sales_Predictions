# Overview

This project is a sales prediction for food items sold at various stores. Throughout this project I will clean the data, build several data visualizations to help understand 
trends in the data. Statiscal analsis which included building models such as Linear Regression, Decision Tree, Bagged Tree and Random Forest were performed to
evaluate predicted sales. These models would give us the Coefficient of Determination(R^2), Mean Absolute Error(MAE), Mean Squared Error(MSE) and Root Mean Squared Error(RMSE).

The model results are:

Linear Regression Coefficient of Determination Training(R^2): 0.5605674972816823

Linear Regression Coefficient of Determination Training(R^2): 0.565852830468762

Decision Tree Coefficient of Determination Training(R^2): 0.6039335724587842

Decision Tree Coefficient of Determination Training(R^2): 0.5947071437341442

Bagged Tree Coefficient of Determination Training(R^2): 0.918204518459746

Bagged Tree Coefficient of Determination Training(R^2): 0.5213957056291549

Random Forests Coefficient of Determination Training(R^2): 0.6105371373976064

Random Forests Coefficient of Determination Training(R^2): 0.6025520510628769


Linear Regression Root Mean Squared Error Training: 1140.3863498499568

Linear Regression Root Mean Squared Error Testing: 1094.4414924070775


Decision Tree Root Mean Squared Error Training: 1082.6546302299298

Decision Tree Root Mean Squared Error Testing: 1057.4468238865645


Bagged Tree Root Mean Squared Error Training: 492.0062036690201

Bagged Tree Root Mean Squared Error Testing: 1149.1119954190244


Random Forests Root Mean Squared Error Training: 1073.5912119749757

Random Forests Root Mean Squared Error Testing: 1047.1627687245482

Based off of the results of the RMSE and R^2 Random Forests Tree would be our best model. Through more analsis of each model the majority of the features in the Decision Tree, Bagged Tree and Random Forest models had no impact on the model. This made the linear regression the most accurate model because of it's utization of every feature in determining the R^2 and RMSE values. 

# Data Dictionary for this dataset

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
