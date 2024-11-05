# 📊 Online Retail Customer Segmentation Project

## 📋 Project Overview
This project is dedicated to **segmenting customers** for an online retail business by leveraging **RFM Analysis** . The objective is to group customers based on their purchase behavior, enabling tailored marketing strategies to increase sales and enhance customer retention. This analysis focuses specifically on the United Kingdom but can be extended to other regions.

## 🧹 Data Cleaning and Preparation
1. **Data Loading**: The dataset is loaded and examined to check its structure, size, and any missing values.
2. **Data Cleaning**:
   - 🔄 **Removed canceled orders** identified by invoice numbers starting with "C".
   - 🧩 **Filtered transactions** with zero or negative values and dropped duplicate entries.
   - ✏️ **Column Formatting**: Cleaned up text (e.g., formatted descriptions to lowercase, removed special characters).
3. **Feature Engineering**:
   - Added new columns for `Total_amount` (Quantity x UnitPrice), `Month`, `Year`, `Week_day`, `Quarter`, and `Hour`.
   - Calculated `Total_amount` for each purchase, crucial for RFM analysis.

## 📊 Exploratory Data Analysis (EDA)
1. **Top 10 Products**: Listed the top-selling items by quantity.
2. **Weekly Sales Patterns**: Analyzed revenue across days, revealing Thursday as the highest-earning day and Sunday as the lowest.
3. **Quarterly Trends**: Visualized revenue trends by quarter to find high and low-performing periods.
4. **Customer and Country Insights**:
   - 🌎 **Top Countries**: Identified the top 10 countries with the most orders.
   - 👤 **Top Customers**: Found the highest revenue-generating customers.

## 📈 RFM Analysis
- **Recency, Frequency, Monetary (RFM) Metrics**: Calculated the `recency`, `frequency`, and `monetary_value` metrics for each customer.
- **Distribution Visualization**: Showcased the distribution of each RFM metric to understand purchasing behaviors.

## 🔍 K-Means Clustering
1. **Data Scaling**: Standardized the RFM features to optimize clustering.
2. **Elbow Method**: Utilized to determine the optimal number of clusters.
3. **K-Means Clustering**: Applied K-Means with five clusters, labeling customers by their cluster group.
4. **Silhouette Score**: Evaluated the clustering performance with a silhouette score.
5. **3D Visualization**: Displayed clusters in a 3D plot to better understand customer segmentation.

## 🎯 Cluster Analysis and Business Solutions
Each of the five customer clusters was analyzed to develop targeted strategies:

### 🔹 Cluster 0 - Moderate Buyers with High Recency
- **Strategy**: Re-engagement Campaigns
- **Actions**: Send personalized emails or moderate discounts to encourage repeat purchases.

### 🔹 Cluster 1 - High-Frequency, High-Value Customers
- **Strategy**: Loyalty and Upsell Programs
- **Actions**: Offer exclusive rewards, upsell premium products, and create VIP engagement events.

### 🔹 Cluster 2 - Recent, High-Value but Moderate Frequency Buyers
- **Strategy**: High-Value Customer Retention
- **Actions**: Provide personalized high-value product offers and periodic purchase reminders.

### 🔹 Cluster 3 - Moderate Recency, Frequency, and Value
- **Strategy**: Incentivize Loyalty and Frequency
- **Actions**: Implement a loyalty program with small perks and send helpful product usage tips.

### 🔹 Cluster 4 - Low Frequency, High Value
- **Strategy**: Encourage Frequency through Targeted Incentives
- **Actions**: Offer strong discounts to reactivate their purchases and recommend high-value items.

## 🚀 Future Work
This segmentation can be expanded to other regions and adapted for specific time frames, promotions, or seasonal insights. Further customer insights can also be developed by monitoring and analyzing the effectiveness of these targeted strategies.

---

Feel free to add or adjust any parts to align with your project details or personal touch! 😊
