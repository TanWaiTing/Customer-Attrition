# Bank Customer Attrition Prediction
In today's competitive banking landscape, customer retention is a key challenge. Banks invest significant resources in acquiring new customers, but retaining existing ones is just as crucial for long-term profitability. Understanding why customers leave and predicting those at risk can help financial institutions take proactive measures to improve customer satisfaction and reduce attrition.
1. We will identify key factors that contribute to customer attrition. The analysis on customer data and attrition patterns will provide actionable insights on the areas for improvement to help bank improve retention strategies.
2. We will build model that predicts customer attrition by classifying customers as "likely to exit" or "likely to stay", enabling the bank to take preemptive actions to retain valuable customers.

## Dataset 
Dataset for Bank Customer Attrition Insights extracted from https://www.kaggle.com/datasets/marusagar/bank-customer-attrition-insights/data

## Data Dictionary 
Target Variable: 

| name | description |
| ---    | --- |
| Exited | "Exited" column indicates whether a customer has left the bank (1) or remained (0).  

Features (Financial): 

| name | description |
| ---    | --- |
| CreditScore | "CreditScore" defines the credit history of the customer.  
| Balance | "Balance" column reflects the amount of money a customer holds in their bank account. 
| EstimatedSalary | "EstimatedSalary" represents the customer’s estimated annual salary. 
| Card Type | "Card Type" refers to the type of credit card a customer holds, such as a standard, premium, or rewards card. 
| Point Earned | "Point Earned" shows the loyalty points a customer has accumulated through the use of their credit card. 

Features (Demographic): 

| name | description |
| ---    | --- |
| Geography | "Geography" refers to the geographical location of the customer. 
| Gender | "Gender" defines the gender of the customer.  
| Age | "Age" is the age of the customer. 

Features (Behavioral): 

| name | description |
| ---    | --- |
| Tenure | "Tenure" refers to the number of years a customer has been with the bank. 
| NumOfProducts | "NumOfProducts" refers to the number of products (e.g., savings accounts, loans, credit cards) that a customer has with the bank. 
| HasCrCard | "HasCrCard" indicates whether or not a customer holds a credit card with the bank. 
| IsActiveMember | "IsActiveMember" column indicates whether a customer actively engages with the bank's services. 
| Complain | "Complain" column shows whether or not a customer has filed a complaint with the bank. 
| Satisfaction Score | "Satisfaction Score" represents how satisfied a customer is with the bank's complaint resolution process. 

Features (Others): 

| name | description |
| ---    | --- |
| RowNumber | "RowNumber" column corresponds to the unique record number for each customer entry. 
| CustomerId | "CustomerId" column consists of randomly generated identifiers for each customer. 
| Surname | "Surname" column holds the last names of customers. 

Features (Added): 

| name | description |
| ---    | --- |
| CreditScoreCategory | "CreditScore" values that are segmented into bins and assigned to numeric labels. 1 = 350-500, 2 = 501-650, 3 = 651-750, 4 = 751-850.
| CreditScoreCategoryLabel | "CreditScoreCategory" values that are assigned to labels. Low = 1, Mid = 2, High = 3, Very High = 4.
| HasBalance | "Balance" values that are converted into bins of whether customer holds balance in their bank account and assigned to numeric labels. 0 = No Balance, 1 = Have Balance.
| BalanceEstSalaryRatio | "BalanceEstSalaryRatio" indicate how financially engaged the customer is with the bank.
| AgeCategoryLabel | "Age" values that are segmented into bins and then assigned to labels. 18-29, 30-39, 40-49, 50-59, 60-69, 70-79, 80+.
| AgeCategory | "AgeCategoryLabel" values that are assigned to numeric labels. 1 = 18-29, 2 = 30-39, 3 = 40-49, 4 = 50-59, 5 = 60-69, 6 = 70-79, 7 = 80+.
| TenureCategory | "Tenure" values that are segmented into bins and then assigned to numeric labels. 1 = 0-2, 2 = 3-7, 3 = 8-10.
| BalPerProduct | "BalPerProduct" indicate how much balance the customer holds on average per product they own.
| EstSalaryToProductRatio | "EstSalaryToProductRatio" shows the affordability of products.
| ActiveBalance | "ActiveBalance" capture active customers with high balances. 
