# Predicting-Customer-Churn
## Introduction
Problem Statement
The company has noticed an increase in the number of customers that have stropped using it’s services. Therefore we have undertaken this project to predict customers at risk of churn. 

What is customer churn?
Customer churn is when your customers chooses to stop using your products or services. This can lead to a Negative brand image, higher customer Acquisition cost and a negative impact on Company Growth.

Importance of Study
Once the company is able to identify the customers at risk of churn they will be able to:
1. Form a better marketing strategy
2. Offer a suitable product mix
3. Revise pricing for services
4. Create a reward progaram for loyal customers
5. Improve the overall customer experience 
6. Increase Customer Retention


## Use Case for Churn Prediction
* Target Variable = CHURN (Yes/No)
* Industry/company = Telecommunication/Telco
* Data Source = Kaggle
* Objective 
    - Understand and Predict customers at risk of churn
    - Identify significant features that can help understand churn


## Project Approach
1. Loaded 3 different csv files into a single dataframe
2. Performed EDA to identify patterns 
3. Feature Enginering and Feature Selection
    - Logistic Regression for feature selection 
4. Model development and Testing, Grid Search, Pipeline Model
5. Model deployment on FLASK 

# Results
## EDA
1. Customers churned are 27% and customers not churned are 73% in the dataset.
2. Gender does not play a role in churn as the difference between male and female churned customers is significantly low. 
3. Customers that don't have partners and dependends are more likely to churn. Why is this because they might have a higher disposable income to spend on telecommunication services?
4. Customers who are on a month-to-month contract and paying via electronic check are churning at the highest rate.
5. The company offers a number of services. Customers who use these services are churning across all of them. This could indicate a poor service, poor customer experience or high price of services. 

## Significant Features
The study stated with aroung 20 features based on the dataset. By running a logistic regression, we were able to narrow down 12 fetures that proved to be significant for predicting churn in this dataset. 

## Modelling 
After creating and testing out a number of models (both manually and using pipeline), the Logistic Regression proved to be the best model with a 78.72% Accuracy score on our test dataset. 

## FLASK
We used FLASK to create a web application for the finalized model. Using test data as a JSON Script we are successfully able to replicate a scenario where there is a customer who is at the risk of churn and one test data for a customer who is not going to churn. 


# Recommendation
By using the results of this project the company needs to establish check and balances for monitoring customer sentiment. Incase a customer has churned, the company should enquire more about why did that customer churned. 

At the end 0% churn rate is impossible to achieve in a real world, but the objective of business is to keep it as low as possible. 







