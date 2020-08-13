# Online Retailer Sales Clustering: Project Overview
* Created this tool to cluster the retail customers of online store. In business it is very important to know about your customers (like one time buyers, long term customers etc).
* Get data from [Kaggle](https://www.kaggle.com/hellbuoy/online-retail-customer-clustering).
* Cleaned data and feature engineering.
* Perform Exploratory Data Analysis.
* Build Model.
## Code and Resources Used
**Python Version:** 3.7 <br>
**Packages:** numpy, pandas, seaborn, matplotlib, plotly, geopy, sklearn, pickle
## Data Cleaning and Feature Engineering
Cleaned data by dropping all null values and  created new featurs by grouping same customer Ids for clustering.<br>
**New Created Features:**<br>
* Quantity.
* Last purchase (days).
* Transactions Amount.
* Number of Transactions.
## Exploratory Data Analysis
Looked for sales and revenue from different countries, customer who churned, customer base in each country and seasonal sales and revenue.<br>
**Visuals:**<br>
![visual not found](https://github.com/zeeshan-akram/Online-Retailer-Sales-Clustering/blob/master/customer-each-country.png)
![visual not found](https://github.com/zeeshan-akram/Online-Retailer-Sales-Clustering/blob/master/month-revenue.png)
![visual not found](https://github.com/zeeshan-akram/Online-Retailer-Sales-Clustering/blob/master/year-sales.png)
![visual not found](https://github.com/zeeshan-akram/Online-Retailer-Sales-Clustering/blob/master/weekly-sales.png)
![visual not found](https://github.com/zeeshan-akram/Online-Retailer-Sales-Clustering/blob/master/weekly-revenue.png)
![visual not found](https://github.com/zeeshan-akram/Online-Retailer-Sales-Clustering/blob/master/sold-item-country.png)
![visual not found](https://github.com/zeeshan-akram/Online-Retailer-Sales-Clustering/blob/master/quarter-revenue.png)
![visual not found](https://github.com/zeeshan-akram/Online-Retailer-Sales-Clustering/blob/master/year-revenue.png)
## Modeling
First I scale down data using standard scaler (where mean = 0, standard deviation = 1). Next find optimal number clusters using Elbow method (4 clusters selected).<br>
At last made inference that which type of customers we have.<br>
![visual not found](https://github.com/zeeshan-akram/Online-Retailer-Sales-Clustering/blob/master/cluster-analysis.png)<br>
**Infrence:**

* ID 2: The people's which made least amount of transaction and also bought least amount of products. It's mean that these peoples are one time buyer's or rarely.
* ID 3: We can call them royal customers because they made highest transaction and bought highest amount of product. It's mean that they are satisfied with products.
* ID 0: These people are the ofenly visitors or we can say they are not satisfied and not too much dishearted with products.
* ID 1: These people just lie behind the royal customers. They are somehow satisfied with products.
##### Number of customers
![visual not found](https://github.com/zeeshan-akram/Online-Retailer-Sales-Clustering/blob/master/customer-each-category.png)
