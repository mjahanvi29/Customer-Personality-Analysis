# Customer-Personality-Analysis

## Contents
1. [Introduction](#introduction)  
2. [Dataset](#dataset)  
3. [Methodology](#methodology)  
   - [Data Preprocessing](#data-preprocessing)  
   - [RFM Analysis](#rfm-analysis)  
   - [Clustering](#clustering)  
   - [Classification](#classification)  
4. [Conclusion](#conclusion)

---

## Introduction
The Customer Personality Analysis project aims to decode consumer behavior using a comprehensive dataset that captures various customer attributes. Understanding customer profiles is essential in making data-driven decisions, optimizing marketing strategies, and enhancing overall customer experience.

The dataset covers demographic details, purchasing patterns, promotion responsiveness, and online interactions, providing a holistic view of customer engagement. This analysis leverages various analytical techniques such as Recency, Frequency, Monetary (RFM) analysis, clustering, and classification to effectively categorize customers into meaningful segments, paving the way for tailored marketing strategies and customer retention initiatives.

---

## Dataset
The dataset is structured into four categories:

### People
- **ID:** Unique customer identifier.  
- **Year_Birth:** Customer's birth year.  
- **Education:** Customer's education level.  
- **Marital_Status:** Customer's marital status.  
- **Income:** Customer's yearly household income.  
- **Kidhome:** Number of children in the household.  
- **Teenhome:** Number of teenagers in the household.  
- **Dt_Customer:** Customer enrollment date.  
- **Recency:** Days since the last purchase.  
- **Complain:** Indicator of complaints in the last 2 years.

### Products
- **MntWines:** Amount spent on wine.  
- **MntFruits:** Amount spent on fruits.  
- **MntMeatProducts:** Amount spent on meat.  
- **MntFishProducts:** Amount spent on fish.  
- **MntSweetProducts:** Amount spent on sweets.  
- **MntGoldProds:** Amount spent on gold.

### Promotion
- **NumDealsPurchases:** Purchases made with discounts.  
- **AcceptedCmp1-5:** Acceptance of offers in campaigns.  
- **Response:** Response to the last campaign.

### Place
- **NumWebPurchases:** Online purchases.  
- **NumCatalogPurchases:** Catalog-based purchases.  
- **NumStorePurchases:** In-store purchases.  
- **NumWebVisitsMonth:** Website visits in the last month.

---

## Methodology

### Data Preprocessing
The initial stage involves:
- Handling missing values and outliers.  
- Standardizing numerical features, encoding categorical variables, and converting date fields.  
- Removing unnecessary columns to improve data quality.

### RFM Analysis
RFM Analysis is used to categorize customers based on:  
- **Recency:** Last purchase date.  
- **Frequency:** Number of transactions.  
- **Monetary:** Total spending.

RFM scores enable identification of high-value customers, providing insights for targeted marketing strategies.

### Clustering
Using **K-means clustering**, customers are grouped based on their RFM scores. The elbow method determines the optimal number of clusters. The main segments identified include:
- **Loyal Customers:** Frequent recent purchasers.  
- **Potential Loyal Customers:** Previous frequent purchasers who have not bought recently.  
- **Churning Customers:** Customers who made recent but infrequent purchases.  
- **Inactive Customers:** Customers with low activity and frequency.

### Classification
The classification stage uses **Support Vector Classification (SVC)** to categorize customers into the identified clusters with high accuracy. This predictive model aids in understanding the likelihood of customers belonging to specific segments.

---

## Conclusion
This project demonstrates the power of customer segmentation using RFM analysis, clustering, and classification. The insights derived enable businesses to implement data-driven marketing strategies, enhance customer retention, and optimize promotional campaigns. Understanding diverse customer segments is key to achieving better engagement and improved customer satisfaction.

