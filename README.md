# Exploratory Data Analysis Telco Customer Churn

![telco customer](https://github.com/Rizal-A/EDA-Telco_Customer_Churn/blob/main/assets/telco%20customer.png)

This is a Exploratory Data Analysis of the Telco Customer Churn.

This public dataset was obtained from Kaggle Dataset [Dataset Telco Customer Churn](https://www.kaggle.com/datasets/blastchar/telco-customer-churn) thanks to BLASTCHAR

**The data set includes information about:**

1. Customers who left within the last month – the column is called Churn
2. Services that each customer has signed up for – phone, multiple lines, internet, online security, online backup, device protection, tech support, and streaming TV and movies
3. Customer account information – how long they’ve been a customer, contract, payment method, paperless billing, monthly charges, and total charges
4. Demographic info about customers – gender, age range, and if they have partners and dependents

**The dataset consists of several features, such as:**

1. customerID : Customer Id
2. gender : Customer Gender ("Male, Female")
3. SeniorCitizen : whether the senior customer (1:"Yes"|0:"No") 
4. Partner : whether the customer has partner ("Yes"|"No")
5. Dependents : whether the customer has Dependents ("Yes"|"No")
6. tenure : length of customer tenure
7. PhoneService : whether the customer has phone service
8. MultipleLines : whether the customer has Multiple Lines
9. InternetService : whether the customer has Internet Service
10. OnlineSecurity : whether the customer has Online Security service
11. OnlineBackup : whether the customer has Online Backup service
12. DeviceProtection : whether the customer has Device Protection service
13. TechSupport : whether the customer has Tech Support service
14. StreamingTV : whether the customer has Streaming TV service
15. StreamingMovies : whether the customer has Streaming Movies service
16. Contract : type of payment contract ("Month to Month", "One Year", "2 Year")
17. PaperlessBilling : the type of bill the customer uses
18. PaymentMethod : type of payment made by the customer
19. MonthlyCharges : customer's monthly bill
20. TotalCharges : customer's total bill
21. Churn : whether the customer Churn ("Yes"|"No")

## The things done on this dataset are

1. Preparation Data
2. Data Cleaning (Missing Values, Duplicated Check)
3. Data Understanding
4. Exploratory Data Analysis
   * Univariate Analysis
   * Bivariate Analysis
   * Multivariate Analysis
   * Deep Dive Exploration
5. EDA Conclusion

## Here the results

1. The dataset in the TotalCharges column, previously the object data type was converted to float, there was an error because it contained a string. After checking it turns out that there is data that contains whitespace strings so that only data that does not contain strings is taken so that the amount of data becomes 7032, after which it is converted to float data type.
2. There is no duplicate data
3. For SeniorCitizen column is discrete data and only has 2 unique values.
4. For the Tenure column, it can be seen that the frequency of distribution is mostly around the number 1 - 5 and the distribution is not normal and the distribution is bimodal.
5. For MonthlyCharges column, the frequency of distribution is mostly around 20 and the distribution is not normal.
6. For the TotalCharges column, the frequency of distribution is mostly between 0 - 200 and the distribution is not normal/symmetrical and tends to skew to the right.
7. There is a strong relationship between tenure and TotalCharges and MonthlyCharges and TotalCharges.
8. It was found that gender and partner do not affect high churn because it can be seen that the number of churn in gender and partner is almost the same.
9. The majority of customers are young because it can be seen that the majority of customers do not have dependents
10. Churn is most prevalent in young customers but based on percentage, it is senior customers who have the highest percentage of churn
11. Churn occurs a lot on tenure 0 - 20 months due to high Monthly Charges and Total Charges, possibly this factor is one of the causes of churn.
12. Churn also occurs in customers who only have 1 - 3 services, this minimal service is the cause of churn and the majority use Fiber Optic internet.
