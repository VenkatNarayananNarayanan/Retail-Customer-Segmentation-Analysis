![image](https://github.com/user-attachments/assets/464487fa-9d82-4829-bb95-420e56da502e)
# Retail-Customer-Segmentation-Analysis

**2. Introduction**
In today's competitive retail environment, understanding customer behavior is crucial for personalized marketing and business growth. This project segments retail customers based on purchasing behavior using Recency, Frequency, and Monetary (RFM) Analysis and K-Means clustering. The results help businesses target the right customers with tailored marketing strategies, ultimately improving customer retention and revenue.

**3. Objective**
The primary objective of this project is to:
✅ Identify distinct customer segments based on purchasing patterns.
✅ Analyze key characteristics of each segment.
✅ Provide data-driven recommendations for customer engagement strategies.
✅ Visualize the findings using Tableau.

**4. Dataset & Preprocessing**
Dataset: Online Retail II UCI from Kaggle( https://www.kaggle.com/datasets/mashlyn/online-retail-ii-uci )

About Dataset:
The dataset used for this analysis consists of transactional data from an online retail business. The key fields in the dataset include:

InvoiceNo – Unique transaction identifier.
CustomerID – Unique identifier for each customer.
InvoiceDate – Date of purchase.
Quantity – Number of items purchased.
UnitPrice – Price per unit.
TotalPrice – Quantity × UnitPrice (computed field).

Preprocessing Steps:
✅ Removed missing CustomerID.
✅ Removed duplicates.
✅ Filtered out negative Quantity (returns).
✅ Removed Outlier using IQR Method. 
✅ Created TotalPrice.

**5. RFM Analysis & Clustering**
RFM Calculation:

Recency (R): How recently a customer made a purchase.
Frequency (F): How often a customer makes purchases.
Monetary (M): Total amount spent by a customer.

Clustering Approach:
✅ Standardized RFM values using StandardScaler.
✅ Applied log transformation to handle skewness
✅ Used Elbow Method to find optimal clusters.
✅ Applied K-Means clustering to segment customers.


**6. Customer Segmentation Insights**
![image](https://github.com/user-attachments/assets/1d28129f-321a-4e35-b1c7-3955fa25252d)


**7. Business Recommendations**
Based on the segmentation, recommended strategies:
VIP Customers : Offer exclusive rewards, early access to sales, and premium support.
Moderately Active Customers : Implement targeted promotions and loyalty points to encourage frequent purchases.
At-Risk Customers: Run re-engagement email campaigns, offering personalized discounts.
One-time Buyers: Provide first-time purchase discounts and improve post-purchase experience to increase retention.

**8. Future Enhancements**
To improve this analysis further, future work could include:
✅ Predictive Analytics: Using machine learning to forecast customer churn.
✅ Behavioral Analysis: Analyzing customer browsing history alongside purchase history.
✅ Integration with Marketing Automation: Implementing real-time customer segmentation in marketing campaigns.

**9. Technologies Used**
Python: Pandas, Scikit-learn, Matplotlib, Seaborn.
SQL: Data extraction and cleaning.
Tableau/Power BI: Dashboard visualizations.

**10. Results & Code**
Find the complete project and dataset on GitHub Repository.
