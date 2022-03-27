# Dream Home Loan Approval Prediction Model
Author: Robert Ramos

## Overview
The data presented in this presentation is loan application data from Dream House loans. The dataset contains includes data that is critical for determining whether an application is approved or denied and also contains data regarding the location of the home and the loan amount requested.

## Variables 
Variables used in analysis

|Variable Name|Description   |   
|---|---|
|Loan_ID|Unique Loan ID| 
|Gender|Male/ Female| 
|Married|Applicant married (Y/N)|
|Dependents|Number of dependents|
|Education|Applicant Education (Graduate/ Under Graduate)| 
|Self_Employed|Self-employed (Y/N)|   
|ApplicantIncome|Applicant income|  
|CoapplicantIncome|Coapplicant income|   
|LoanAmount|Loan amount in thousands|  
|Loan_Amount_Term|Term of the loan in months| 
|Credit_History|Credit history meets guidelines| 
|PropertyArea|Urban/ Semi-Urban/ Rural|

## Methods
See my [Google Colab](https://colab.research.google.com/drive/1-nYMdKYLTlWY7F99ZTBCMHwFgM3eVi0F#scrollTo=gr63uFrBHyFm) for detailed steps I took to obtain, clean and analyze the data. The general steps were:
* Imported raw data from a csv file into a dataframe
* Cleaned data by dropping columns, correcting inconsistant values, imputing missing values and converting columns to appropriate datatypes
* Create visualizations to explore characteristics of products and how they affect sales
* Create machine learning models to find best fit

## Results
### Item Sales by Outlet Type
Supermarket Type1's had the highest volume of item sales over the other 3 types of outlets combined.

![](images/OutletSales.png)
![](images/ItemSalesbyOutletTypes.png)

### Item Sales by Item Category
- Highest selling product categories are Fruits and Vegetables, Snack foods and Household products
- Lowest selling item categories are Breakfast, Seafood and products that fall into the Others category
![](images/ItemSalesbyItemType.png)

## Summary
Based on the data that I have analyzed, items that will sell highest in quantities are those that are sold in Supermarket Type2 outlets and top products categories that are more likely to sell than others are Fruits and Vegetables, Snack foods and Household products.


## Recommendation
* My recommendation to increase future sales of products would be to focus on building more Type 1 supermarkets as this will lead to the highest volume of sales across all products.
* From comparing the two models, the Regression tree model is a better for predicting which product properties can lead to better sales. My justification for this based on the  model metrics is that is that the Decision Tree model has a higher R2 score which means that the training and testing datasets have a higher correlation and well as a lower RMSE which means that the model is more accurate at predicting in comparison to the Linear Regression Model.

![](images/LR.png)
![](images/DTR.png)
