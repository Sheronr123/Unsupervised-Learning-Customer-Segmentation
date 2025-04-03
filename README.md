# Customer Segmentation using K-Means Clustering

## 📌 Overview
This project performs customer segmentation on credit card customer data using K-Means clustering to identify distinct customer groups based on their spending and payment behaviors.

## 📊 Dataset
The dataset contains 8,950 customer records with 18 features including:

| Feature | Description |
|---------|-------------|
| `BALANCE` | Credit card balance |
| `PURCHASES` | Total purchase amount |
| `CASH_ADVANCE` | Cash advance amount |
| `CREDIT_LIMIT` | Customer's credit limit |
| `PAYMENTS` | Payment amounts |
| `TENURE` | Duration as customer (in months) |

## 🔧 Methodology
1. **Data Preprocessing**:
   - Handled missing values
   - Removed highly correlated features
   - Standardized features using `StandardScaler`

2. **Clustering**:
   - Used Elbow Method to determine optimal clusters (k=7)
   - Applied K-Means clustering
   - Silhouette Score: 0.227

3. **Analysis**:
   - Visualized clusters using PCA
   - Analyzed cluster characteristics
   - Developed business recommendations

## 📈 Results
Identified 7 customer segments:

| Cluster | Characteristics |
|---------|-----------------|
| 0 | Potential Revolvers - High balance, frequent cash advances |
| 1 | Transactors - Pays full balance often |
| 2 | VIP Customers - High installment purchases |
| 3 | Moderate Users - Balanced spending |
| 4 | High Spenders - Very high purchases |
| 5 | One-Off Purchasers | 
| 6 | At-Risk Customers - Low activity |

## 💡 Business Applications
- **Targeted Marketing**: Different strategies per segment
- **Customer Retention**: Focus on at-risk segments
- **Risk Management**: Monitor high cash advance users

## 🛠️ Installation
```bash
git clone https://github.com/yourusername/customer-segmentation.git
cd customer-segmentation
pip install -r requirements.txt
