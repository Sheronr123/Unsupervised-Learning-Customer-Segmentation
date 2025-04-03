Customer Segmentation using K-Means Clustering
Overview
This project performs customer segmentation on credit card customer data using K-Means clustering. The goal is to identify distinct groups of customers based on their spending habits, payment behaviors, and credit usage patterns. These segments can then be used for targeted marketing, customer retention strategies, and business decision-making.

Dataset
The dataset contains 8,950 customer records with 18 features including:

BALANCE: Credit card balance

PURCHASES: Total purchase amount

CASH_ADVANCE: Cash advance amount

CREDIT_LIMIT: Customer's credit limit

PAYMENTS: Payment amounts

TENURE: Duration as customer (in months)

Methodology
Data Preprocessing:

Handled missing values (imputed median for MINIMUM_PAYMENTS, mode for CREDIT_LIMIT)

Removed highly correlated features

Standardized features using StandardScaler

Clustering:

Used the Elbow Method to determine optimal number of clusters (k=7)

Applied K-Means clustering

Evaluated with Silhouette Score (0.227)

Analysis:

Visualized clusters using PCA (Principal Component Analysis)

Analyzed cluster characteristics

Developed business recommendations for each segment

Key Findings
The analysis identified 7 distinct customer segments:

Potential Revolvers: High balance, frequent cash advances

Transactors: Low cash advance usage, often pays full balance

VIP Customers: High installment purchases

Moderate Users: Balanced spending patterns

High Spenders: Very high purchases and credit limits

One-Off Purchasers: Frequent single purchases

At-Risk Customers: Low activity and spending

Business Applications
Targeted Marketing: Different strategies for each segment

Customer Retention: Focus on at-risk segments

Credit Risk Management: Monitor high cash advance users

Product Development: Create features for specific segments

Files
Customer_Data.csv: Input dataset

Customer_Segmentation.ipynb: Jupyter notebook with full analysis

Requirements
Python 3.x

Libraries: pandas, numpy, matplotlib, seaborn, scikit-learn

How to Run
Install required packages: pip install -r requirements.txt

Run the Jupyter notebook: jupyter notebook Customer_Segmentation.ipynb

Future Work
Experiment with other clustering algorithms (DBSCAN, Hierarchical)

Incorporate more features for richer segmentation

Develop real-time customer segmentation system


