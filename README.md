# Customer_Segmentation_Clustering

## Table of Contents
1. Context
2. Importing libraries
3. About the dataset
4. Loading Data
5. Data Cleaning
6. Data Preprocessing
7. Dimensionality Reduction
8. Clustering
9. Evaluation models
10. Cluster Profiling
11. Conclusion

## Context
In this project, I have performed an unsupervised clustering of data on the customer's records from a groceries firm's database. Customer segmentation is the practice of separating customers into groups that reflect similarities among customers in each cluster. I have divided customers into segments to optimize the significance of each customer to the business and to modify products according to distinct needs and behaviours of the customers. It also helps the business to cater to the concerns of different types of customers.

## About the dataset

**People**

* ID: Customer's unique identifier
* Year_Birth: Customer's birth year
* Education: Customer's education level
* Marital_Status: Customer's marital status
* Income: Customer's yearly household income
* Kidhome: Number of children in customer's household
* Teenhome: Number of teenagers in customer's household
* Dt_Customer: Date of customer's enrollment with the company
* Recency: Number of days since customer's last purchase
* Complain: 1 if the customer complained in the last 2 years, 0 otherwise

**Products**

* MntWines: Amount spent on wine in last 2 years
* MntFruits: Amount spent on fruits in last 2 years
* MntMeatProducts: Amount spent on meat in last 2 years
* MntFishProducts: Amount spent on fish in last 2 years
* MntSweetProducts: Amount spent on sweets in last 2 years
* MntGoldProds: Amount spent on gold in last 2 years
Promotion


**NumDealsPurchases: Number of purchases made with a discount**

* AcceptedCmp1: 1 if customer accepted the offer in the 1st campaign, 0 otherwise
* AcceptedCmp2: 1 if customer accepted the offer in the 2nd campaign, 0 otherwise
* AcceptedCmp3: 1 if customer accepted the offer in the 3rd campaign, 0 otherwise
* AcceptedCmp4: 1 if customer accepted the offer in the 4th campaign, 0 otherwise
* AcceptedCmp5: 1 if customer accepted the offer in the 5th campaign, 0 otherwise
* Response: 1 if customer accepted the offer in the last campaign, 0 otherwise

**Place**

* NumWebPurchases: Number of purchases made through the company’s website
* NumCatalogPurchases: Number of purchases made using a catalogue
* NumStorePurchases: Number of purchases made directly in stores
* NumWebVisitsMonth: Number of visits to company’s website in the last month

## Cluster Profiling

| Name   |Cluster-0   |Cluster-1   |Cluster-2   |Cluster-3  |
|--------|------------|------------|------------|-----------|
|   Age  |   40-80    |    30-50   |   40-80    |20-30 , 80-100|
|Income  |  40K-60K   |   <40K     |  60K-80K   |   >80K    |
| Spent  |   <600     |   <400     |    >600    |   >800    |
| Kid at home | mostly 2 kid | mostly 1 kid | no kid |no kid |
|Teen at home |  1-2 teen    |   1 teen     | no teen|no teen|
|  Children   |      2-3     |   mostly 1   | mostly 1 |  0  |
| family size |      4-5     |      2-3     | 2-3    |  1-2  |
| is parent ? | definitely parent | some are parent | definitely parent |  they are not parent  |
