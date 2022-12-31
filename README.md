# Advertising and Sales

## Introduction

This dataset contains the advertising expenses of a company through different mediums which are TV, Radio and Newspaper. We also know the sales of the company which is the target variables. 

In this project we are building a ML Regression model to predict the sales of the company depending on the advertising expenses. We need to figure out the statistically significant variables so inferences can be drawn on unseen data. 

## Business Goals 

Predict the sales price of the company from the advertising expenses through the right channel so it does not lead to faulty use or distribution of company funds in the advertising medium.  

## Data Dictionary 

  * TV - Cost through TV advertisement
Radio - Cost through Radio advertisement
Newspaper - Cost through Newspaper advertisement 
Sales - Sales generated 

## Approach 

### 1. Data Source 
[Link](https://www.kaggle.com/datasets/ashydv/advertising-dataset)

### 2. Data Import 
- Reading and Understanding the data 

### 3. Data Visualization 
- Correlations between the independent and target variable was found 
- TV being highly correlated with the target variable 

### 4. Model Building without scaling the variables and after scaling the variables
- Data splitting into train and test sets 
- Model was built using Linear Regression algorithm 
- Model was also built using Orinary Least Square method from statsmodels to find the siginifance of the varibales and model fit. 
- Variables with p-value > 0.05 removed. 

### 5. Residual Analysis
- Validating the initial assumption of normal distribution of residuals and zero mean

### 6. Model Prediction 
- Prediction on the test set was done with the remaining variables that are TV and Radio. 
- Evaluation metrics were calculated to check the performance of the model. 

**Equation of Best fit line**
**Sales = (0.659537 * TV) + (0.229966 * Radio) + 0.085545**

<img width="324" alt="Screenshot 2022-12-31 at 11 57 24 PM" src="https://user-images.githubusercontent.com/31815562/210152604-0e3f0a64-2c4b-42f2-8449-1493fe13eb30.png">

<img width="562" alt="Screenshot 2022-12-31 at 11 58 26 PM" src="https://user-images.githubusercontent.com/31815562/210152631-657ef890-1e8e-4ba0-90ab-454a9577caeb.png">
