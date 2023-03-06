# Credit-Card-Default-Prediction

#### Introduction

For the banking and credit card industries, credit risk has typically been the biggest risk and the one that requires the most capital. Statistics and business reports from the sector can support this. For instance, "The Reserve Bank of India bases its assessment of credit card delinquencies on the proportion of accounts that are at least 90 days overdue. The key to increasing revenue and decreasing loss for the banking and credit card industries is therefore analysing, recognising, and controlling default risk.
The purpose of this project is to conduct quantitative analysis on credit card default risk by using interpretable machine learning models with accessible customer data, instead of credit score or credit history, with the goal of assisting and speeding up the human decision-making process.

#### Problem Statement

This project is aimed at predicting the case of customers default payments in Taiwan. From the perspective of risk management, the result of predictive accuracy of the estimated probability of default will be more valuable than the binary result of classification - credible or not credible clients. We can use the K-S chart to evaluate which customers will default on their credit card payments.

#### Model Comparisons

Compare within the 3 models: Logistic Regression has the highest recall but also the lowest precision. Random Forest outperforms Logistic Regression and XGBoost if
measured on their F1 scores, which is the balance between precision and recall.XGBoost has a decent performance but it takes the most time to tune the model.

![image](https://user-images.githubusercontent.com/78267410/223168618-548d0b9d-dc6c-452f-b75c-2bf10b6f79e7.png)

#### Conclusions

Based on the exploratory data analysis, we discover that human characteristics are not the most important predictors of default, the payment status of the most 2 months and credit limit are. From the modeling, we are able to classify default risk with accessible customer data and find a decent model.

 Suggestions: With every classification model, there is a general trade-off between precision and recall. A model’s recall can be adjusted to arbitrarily high at the cost of lower precision. 

Below is our suggested recall plot. Note the threshold can be adjusted to reach highe Recall.
![image](https://user-images.githubusercontent.com/78267410/223169276-9a1f846f-b6e2-4fe8-aaa3-ac3fe5b7e20a.png)

● Limitations: The dataset only includes 30,000 records of non-American consumers,there might be differences between US consumers and non-US consumers. Even with
the best model Random Forest, we can only detect 51.5% of default customers, and among those that are being flagged as default, only 51.2% of them indeed have default.


