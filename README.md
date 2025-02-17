![image](https://github.com/user-attachments/assets/464487fa-9d82-4829-bb95-420e56da502e)
# Retail-Customer-Segmentation-Analysis

**1. Introduction**

In today's competitive retail environment, understanding customer behavior is crucial for personalized marketing and business growth. This project utilizes the Online Retail II UCI dataset from Kaggle, which contains transactional data from a UK-based online retail store between 2009-2011. The project segments customers based on Recency, Frequency, and Monetary (RFM) analysis using SQL, Python, and Tableau. The purpose is to help businesses identify customer segments, understand their purchasing patterns, and create targeted marketing strategies to improve retention and revenue.

**2. Objective**

The primary objective of this project is to:

✅ Identify distinct customer segments based on purchasing patterns.

✅ Analyze key characteristics of each segment.

✅ Provide data-driven recommendations for customer engagement strategies.

✅ Visualize the findings using Tableau.

**3. Dataset & Preprocessing**

Dataset: Online Retail II UCI from Kaggle( https://www.kaggle.com/datasets/mashlyn/online-retail-ii-uci )

About Dataset:
The dataset used for this analysis is the Online Retail II UCI dataset from Kaggle (https://www.kaggle.com/datasets/mashlyn/online-retail-ii-uci).
It consists of transactional data from a UK-based online retailer, covering the period from 2009 to 2011. Key fields include:

InvoiceNo – Unique transaction identifier.
StockCode – Unique product identifier.
Description – Product name.
Quantity – Number of products purchased.
InvoiceDate – Date and time of the transaction.
UnitPrice – Price per unit.
CustomerID – Unique identifier for each customer.
Country – Country where the customer resides.

This dataset was processed to calculate RFM metrics, which formed the basis for customer segmentation.

Preprocessing Steps:

✅ Removed missing CustomerID.

✅ Removed duplicates.

✅ Filtered out negative Quantity (returns).

✅ Removed Outlier using IQR Method. 

✅ Created TotalPrice.

SQL Database Integration:

The dataset was first inserted into an SQL database.
RFM metrics were calculated directly in SQL:

Recency: Difference between the last transaction date and the most recent date in the dataset.
Frequency: Count of unique transactions per customer.
Monetary: Sum of TotalPrice per customer.

The extracted RFM metrics were then fetched into Jupyter Notebook for further analysis.

**4. RFM Analysis & Clustering**

RFM Calculation:

Recency (R): How recently a customer made a purchase.
Frequency (F): How often a customer makes purchases.
Monetary (M): Total amount spent by a customer.

Clustering Approach:

✅ Standardized RFM values using StandardScaler.

✅ Applied log transformation to handle skewness.

✅ Used Elbow Method to find optimal clusters.

✅ Applied K-Means clustering to segment customers.


**5. Customer Segmentation Insights**

![image](https://github.com/user-attachments/assets/1d28129f-321a-4e35-b1c7-3955fa25252d)

**6. Data Visualization in Tableau**

Key dashboards created:

RFM Heatmap: Visual representation of RFM scores.
Customer Lifetime Value: Bar chart showing CLV across customers.
Recency vs. Monetary and Frequency vs. Monetary: Scatter plots highlighting segment differences.
Segment Distribution: Pie chart showing customer segment proportions.

**7. Business Recommendations**

Based on the segmentation, recommended strategies:
VIP Customers : Offer exclusive rewards, early access to sales, and premium support.
Moderately Active Customers : Implement targeted promotions and loyalty points to encourage frequent purchases.
At-Risk Customers: Run re-engagement email campaigns, offering personalized discounts.
One-time Buyers: Provide first-time purchase discounts and improve post-purchase experience to increase retention.

**8. Conclusion**

This project successfully segmented retail customers using the Online Retail II UCI dataset from Kaggle. RFM analysis provided a comprehensive understanding of customer purchasing behavior, and K-Means clustering allowed for meaningful segmentation. The resulting insights enable businesses to implement personalized marketing strategies, improve customer engagement, and boost revenue. This project also highlights the importance of data-driven decision-making in modern retail.

**9. Future Enhancements**

To improve this analysis further, future work could include:

✅ Predictive Analytics: Using machine learning to forecast customer churn.

✅ Behavioral Analysis: Analyzing customer browsing history alongside purchase history.

✅ Integration with Marketing Automation: Implementing real-time customer segmentation in marketing campaigns.

**10. Technologies Used**

Python: Data extraction, preprocessing(Pandas, Scikit-learn, Matplotlib, Seaborn) and K-mean clustering
SQL: Data storage and RFM metric calculations.
Tableau: Dashboard visualizations.

**11. Results & Code**

Find the complete project and dataset on GitHub Repository(https://github.com/VenkatNarayananNarayanan/Retail-Customer-Segmentation-Analysis/tree/main).
