# Introduction

**Background**

ConnectTel is a leading telecommunications company that has been providing cutting-edge services to its diverse customer base. In an ever-evolving industry, customer retention is a key focus for ConnectTel to sustain its market position. Understanding and predicting customer churn has become a vital aspect of their business strategy.

Customer churn occurs when subscribers discontinue using ConnectTel's services. To quantify this, ConnectTel calculates its churn rate by dividing the number of lost customers during a specific period (e.g., a quarter) by the total number of customers at the beginning of that period. This metric helps the company assess the health of its customer base and strategize on measures to minimize churn.


**Problem Statement**

In the rapidly evolving telecommunications industry, ConnectTel is confronted with the critical challenge of customer churn, where subscribers opt to discontinue their services. To maintain its leadership and navigate market dynamics successfully, ConnectTel recognizes the paramount importance of customer retention as a core element of its business strategy.


**Objective**

ConnectTel aims to harness the power of machine learning to develop a predictive model capable of identifying potential customer churn. The primary focus is on avoiding misidentification, ensuring that customers with a propensity to churn are accurately identified as such and not incorrectly labeled as non-churn customers.

**Dataset**

Kaggle - Telco Customer Churn

https://www.kaggle.com/datasets/blastchar/telco-customer-churn/data

- `customerID` - Customer ID

- `gender` - Whether the customer is a male or a female

- `SeniorCitizen` - Whether the customer is a senior citizen (1, 0)

- `Partner` - Whether the customer has a partner (Yes, No)

- `Dependents` - Whether the customer has dependents (Yes, No)

- `tenure` - Number of months the customer has stayed with the company

- `PhoneService` - Whether the customer has a phone service (Yes, No)

- `MultipleLines` - Whether the customer has multiple lines (Yes, No, No phone service)

- `InternetService` - Customer’s internet service provider (DSL, Fiber optic, No)

- `OnlineSecurity` - Whether the customer has online security (Yes, No, No internet service)

- `OnlineBackup` - Whether the customer has online backup or not (Yes, No, No internet service)

- `DeviceProtection` - Whether the customer has device protection (Yes, No, No internet service)

- `TechSupport` - Whether the customer has tech support (Yes, No, No internet service)

- `StreamingTV` - Whether the customer has streaming TV service (Yes, No, No internet service)

- `StreamingMovies` - Whether the customer has streaming movies service (Yes, No, No internet service)

- `Contract` - Indicates the type of the contract (Month-to-month, One year, Two year)

- `PaperlessBilling` - Whether the customer has paperless billing (Yes, No)

- `PaymentMethod` - Indicates the payment method (Electronic check, Mailed check, Bank transfer (automatic), Credit card (automatic))

- `MonthlyCharges` - Indicates the current monthly subscription cost of the customer

- `TotalCharges` - Indicates the total charges paid by the customer so far

- `Churn` - Indicates whether the customer churned


# Conclusion
As a data scientist at ConnectTel, I successfully developed a predictive model with a focus on minimizing false predictions for customers who are likely to churn. 

The GradientBoosting model, after tuning and feature selection, showed the best overall performance with a recall score of 86%.However, the model exhibits weaknesses in predicting customers who should not churn. Significant variables in this model include contract month-to-month, tenure, monthly charges, senior citizen, and paperless billing.

The model can be further enhanced to improve precision by incorporating additional features. Additionally, addressing class imbalance can involve trying alternative methods such as SMOTENC. Exploring different ensemble models, such as XGBoost, may provide diversity and improve overall performance. Lastly, implementing regularization techniques can help manage overfitting and contribute to precision improvement.


# Recomendation to Business

Establish real-time churn alerts based on the predictive model to notify your team efficiently when a customer is at risk of churning. This allows quick intervention for customer retention. Exercise caution, especially in cases of predicted false negatives, as inaccuracies may occur. Regularly review and refine the alert system for improved accuracy and relevance in real-world scenarios.

**Contract Month-to-Month**:

Offer incentives or special promotions to encourage customers to switch from month-to-month contracts to long-term contracts. This can improve customer retention.

**Tenure:**

Introduce loyalty programs or exclusive offers for customers who have subscribed for a specific duration. Such efforts can enhance loyalty among long-term subscribers.

**Monthly Charges:**

Consider adjusting pricing or offering service packages to meet customer needs and maintain affordable monthly rates. This can help alleviate financial pressure on customers.

**Senior Citizen:**

Specifically for senior customers, offer additional services or features tailored to their needs. Pay attention to the preferences and comfort of senior customers in communication and interaction with services.

**Paperless Billing_No:**

Educate customers on the benefits and convenience of using paperless billing. Provide incentives or special discounts for customers switching to paperless billing methods.
