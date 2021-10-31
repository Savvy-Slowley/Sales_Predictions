# Overview


WILL BE UPDATED


Data from https://datahack.analyticsvidhya.com/contest/practice-problem-big-mart-sales-iii/.
### Generating and Cleaning the Data
This project is a sales prediction for food items sold at various stores. The first step after generating the data is data cleaning. While I was data cleaning I checked for duplications and then null values. There were no duplications within the data however there were two columns("Outlet_Size" and "Item_Weight") with null values. I started with "Outlet_Size" where I looked for a trend between it and other columns. I realized quickly that "Outlet_Size" and "Outlet_Location_Type" had a relationship between them where  'Tier 3' = 'Medium' ,  'Tier 1' = 'Small' and 'Tier 2' = 'Large'( I changed the word 'High' to 'Large'). For the "Item_Weight" column I made a histogram and saw the weights were evenly distributed and I filled the remaining null values with the mean of "Item_Weight".  I then quickly checked all the value counts for each column to see if there is any data imputed incorrectly. I changed 'low fat' and 'LF' to 'Low Fat'. I also changed 'reg' to 'Regular'. 

### Exploratory Data Analysis
I continue my code doing exploratory data analysis. I found the count, mean, standard deviation, quartiles, minimum, and maximum values of the data. I then created multiple visualizations to understand the data more like "Outlet_Establishment" by "Item_Type" and "Outlet_Size" By "Item_Fat_Content". These visualizations were followed by a heat map where I was able to see the correlations between columns of my data. 

### Building the Models
The pre-processing for the data models continued by dummy encoding categorical variables and dropping columns that were not important as features. I was now able to build a model for the dataset with "Item_Outlet_Sales" as my target. I built models such as Linear Regression, Decision Tree, Bagged Tree, and Random Forest to evaluate predicted sales. These models would give us the Coefficient of Determination(R^2), Mean Absolute Error(MAE), Mean Squared Error(MSE), and Root Mean Squared Error(RMSE). 

## The Model Results
### Coefficient of Determination(R^2)

Linear Regression Coefficient of Determination Training(R^2): 0.5605674972816823

Linear Regression Coefficient of Determination Training(R^2): 0.565852830468762
________________________________________________________________________________________________________________________________________________________________________________
Decision Tree Coefficient of Determination Training(R^2): 0.6039335724587842

Decision Tree Coefficient of Determination Training(R^2): 0.5947071437341442
________________________________________________________________________________________________________________________________________________________________________________
Bagged Tree Coefficient of Determination Training(R^2): 0.918204518459746

Bagged Tree Coefficient of Determination Training(R^2): 0.5213957056291549
________________________________________________________________________________________________________________________________________________________________________________
Random Forests Coefficient of Determination Training(R^2): 0.6105371373976064

Random Forests Coefficient of Determination Training(R^2): 0.6025520510628769

________________________________________________________________________________________________________________________________________________________________________________
________________________________________________________________________________________________________________________________________________________________________________
### Root Mean Squared Error(RMSE)

Linear Regression Root Mean Squared Error Training(RMSE): 1140.3863498499568

Linear Regression Root Mean Squared Error Testing(RMSE): 1094.4414924070775
________________________________________________________________________________________________________________________________________________________________________________
Decision Tree Root Mean Squared Error Training(RMSE): 1082.6546302299298

Decision Tree Root Mean Squared Error Testing(RMSE): 1057.4468238865645
________________________________________________________________________________________________________________________________________________________________________________
Bagged Tree Root Mean Squared Error Training(RMSE): 492.0062036690201

Bagged Tree Root Mean Squared Error Testing(RMSE): 1149.1119954190244
________________________________________________________________________________________________________________________________________________________________________________
Random Forests Root Mean Squared Error Training(RMSE): 1073.5912119749757

Random Forests Root Mean Squared Error Testing(RMSE): 1047.1627687245482
________________________________________________________________________________________________________________________________________________________________________________
Based on the results of the RMSE and R^2 Random Forests Tree would be our best model. Through more analysis of each model the majority of the features in the Decision Tree, Bagged Tree, and Random Forest models had no impact on the model. This made the linear regression the most accurate model because it utilizes every feature in determining the R^2 and RMSE values. 


# Data Dictionary for this Dataset

### Variable Name	Descriptions

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
