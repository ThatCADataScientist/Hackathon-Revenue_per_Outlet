# Hackathon-Revenue_per_Outlet
>Analytics Vidhya Hackathon

# Problem Statement
> The data scientists at BigMart have collected 2013 sales data for 1559 products across 10 stores in different cities. Also, certain attributes of each product and store have been defined. The aim is to build a predictive model and predict the sales of each product at a particular outlet.

# About the dataset
The Dataset contains 11 Independent Features and 1 Dependent Feature(Item_Outlet_Sales) which are described as follows-
- Item_Identifier=	Unique product ID
- Item_Weight	Weight= of product
- Item_Fat_Content=	Whether the product is low fat or not
- Item_Visibility=	The % of total display area of all products in a store allocated to the particular product
- Item_Type=	The category to which the product belongs
- Item_MRP=	Maximum Retail Price (list price) of the product
- Outlet_Identifier=	Unique store ID
- Outlet_Establishment_Year=	The year in which store was established
- Outlet_Size=	The size of the store in terms of ground area covered
- Outlet_Location_Type=	The type of city in which the store is located
- Outlet_Type=	Whether the outlet is just a grocery store or some sort of supermarket
- Item_Outlet_Sales=	Sales of the product in the particular store. This is the outcome variable to be predicted.

# Steps used during the project
1) Exploratary Data Analysis- 
  - Correlation with Target Variable
  - Plot to know the Target Variables distribution
  - Distplot to check the skewness of every Continous Feature
  - Stacked Bar plot to know the count of every Categorical Feature
  
 2) Preprocessing and Feature Engineering -
  - Filling missing values. For one feature we applied an Ensemble Voting Classifier to predict values.
  - Dealing with the Skewness of the data by using scalers
  - Scaling the continous columns
  - One hot Encoding on the categorical columns
  
  3) Applying models-
  - The problem is a Regression problem used for prediction
  - Various models were used on the above data
  - The best performing was the Catboost Regressor
  
  4) Evaluation Metric-
   
   - Model performance was evaluated on the basis of the prediction of Outlet_sales and the metric to judge it was Root Mean Squared Error.
   
   - Error for Catboost Classifier- 1189.23263304827
     
     
# Executive Summary
1) Product Segmentation and Advertising -
  Companies spend a handsome amount of money on advertising for enhancing their turnover. Advertising should be considered on products based on their sales and profits per unit and in totality. With this the company can segment and segregate products. They could either use Pareto Analysis (80/20 Rule) for advertising or on the other hand they could increase advertising for low profitable products to enhance their sales.

2) Market Segmentation-
  By doing this they can apply Market Segmentation. Market segmentation gives a clear understanding of the retail customers' requirements. With the clear understanding of market segmentation, the retail managers and marketing personnel can develop strategies to reach out to the customers with specific needs and preferences.
