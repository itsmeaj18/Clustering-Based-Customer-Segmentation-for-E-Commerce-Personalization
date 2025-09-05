# 🛍️ Clustering-Based-Customer-Segmentation-for-E-Commerce-Personalization

## 📂 Dataset
The dataset used in this project can be downloaded from Kaggle:  
🔗 [Sales Simulation Dataset](https://www.kaggle.com/datasets/noeyislearning/sales-simulation)  

Download the dataset and place it in your project directory before running the notebook.

---

## 📌 Project Overview
This project focuses on **customer segmentation** to help businesses personalize marketing, optimize loyalty programs, and reduce churn.  
We use **unsupervised machine learning (clustering)** to group customers into meaningful segments based on their **demographics, purchase behavior, loyalty engagement, discounts, and delivery experience**.

---

## 🎯 Problem Statement
**Cluster customers into meaningful segments based on their demographics, purchase behavior, discounts used, loyalty engagement, delivery experience, and satisfaction ratings — to help businesses personalize marketing strategies, optimize loyalty programs, and reduce churn.**

---

## ⚙️ Methodology
1. **Data Understanding & Cleaning**
   - Checked data types and null values  
   - Converted date/time columns to datetime format  
   - Created derived features (e.g., `membership_duration_days`, `delivery_time_days`, `estimated_vs_actual_delivery`)  

2. **Feature Selection**
   - Removed redundant features (e.g., raw dates, payment times)  
   - Checked multicollinearity with correlation heatmap  
   - Retained informative features for clustering  

3. **Encoding**
   - Manual Encoding: `sex`  
   - One-Hot Encoding: `payment_method`, `product_category`  
   - Binary Encoding: `purchase_medium`, `shipping_method`  

4. **Feature Scaling**
   - StandardScaler applied to numerical features  

5. **Clustering**
   - Algorithm: **KMeans**  
   - Range tested: k = 2 to 30  
   - Evaluation Metrics:  
     - Silhouette Score  
     - Davies-Bouldin Index  
     - Calinski-Harabasz Score  

6. **Cluster Analysis & Naming**
   - Cluster 0 → **High-Spending Loyalists**  
   - Cluster 1 → **Discount Seekers**  
   - Cluster 2 → **Casual Shoppers**  
   - Cluster 3 → **Delivery-Sensitive Customers**  

---

## 📊 Results
- **Optimal Clusters**: 4  
- Each cluster reflects unique behavior patterns  
- Segments provide actionable insights for targeted marketing  

---

## ✅ Recommendations
- **High-Spending Loyalists** → Exclusive rewards, premium loyalty perks  
- **Discount Seekers** → Coupons, flash sales, bundle offers  
- **Casual Shoppers** → Engagement campaigns, personalized recommendations  
- **Delivery-Sensitive Customers** → Faster shipping options, delivery guarantees  
