# E-commerce Analysis
## Table of Content
- [Overview](#overview)
- [Metrics](#metrics)
- [Key Findings](#key-findings)
- [Recommendations](#recommendations)
- [Data Analysis Process](#data-analysis-process)

### Overview
This report presents a comprehensive analysis of a Brazilian E-Commerce dataset, covering over 17 million orders placed between 2016 and 2018. The analysis explores customer behavior, product performance, and payment preferences, offering valuable insights into key trends that influence business growth. Additionally, the report delves into customer satisfaction levels with the delivery system, identifying areas of improvement and success in meeting customer expectations.

![Braz Dashboard 1](https://github.com/user-attachments/assets/2dd8dfed-a3a3-46e5-9b44-dce6d01879c9)

![Braz Dashboard 2](https://github.com/user-attachments/assets/0088ebbf-456d-447d-9d17-be1e6c32294d)

### Metrics
- Total Orders: Count of Orders, Yearly distribution of Orders, Monthly distribution of Orders, Top 10 Product categories
- Total Payment: Total Amount generated from Sales ($)
- Average Delivery Time: Average Delivery Duration (Days)
- Percentage On-time Delivery
- Percentage Delayed Delivery

### Key Findings
- Customer Satisfaction: A majority of customers (58%) rated the services provided as "very good."
- PC games were identified as a Product Category prone to customer dissatisfaction.
- Payment Preferences: Credit cards were the most popular payment method, accounting for 74% of transactions.
- Order Trends: The number of orders has increased steadily from 2016 to 2018, indicating a growing market. Seasonal patterns were observed with higher sales in the middle of the year and lower sales towards the end.
- Delivery Performance: Delayed deliveries were a common complaint among customers who gave poor reviews.
  
### Current Situation
The Brazilian e-commerce market is experiencing growth, but challenges remain in terms of customer satisfaction and delivery efficiency. While the majority of customers are satisfied with the overall experience, there is room for improvement in specific product categories and delivery times.

### Recommendations
To further enhance the e-commerce market, the following recommendations are suggested:
- Targeted Marketing: Implement targeted marketing strategies to capitalize on the seasonal trends observed in order volume.
- Payment Optimization: Improve the payment process, especially for credit cards, to enhance customer convenience and reduce friction.
- Delivery Efficiency: Invest in logistics and delivery infrastructure to ensure timely and reliable deliveries.
- Product Quality Control: Strengthen quality control measures for PC games and other products prone to customer dissatisfaction.
- Deeper Analysis: Product categories with low ratings should be investigated further to understand the reason for customer dissatisfaction.
- Customer Feedback Analysis: Continuously monitor customer feedback to identify areas for improvement and address emerging issues.
By addressing these recommendations, Brazilian e-commerce businesses can enhance customer satisfaction, improve operational efficiency, and drive further growth in the market.

## Data Analysis Process
The dataset comprised of real-time data taken from Olist Store in Brazil. A total of 8 different tables were included in the dataset and each of them contained unique information about the business activities.

The tables include:
- Olist Customer Dataset
- Olist geolocation Dataset
- Olist Order items Dataset
- Olist Order payment
- Order review
- Orders Dataset
- Products Dataset
- Sellers Dataset

Over 17,000,000 orders were recorded between the years 2016 and 2018. These 17,000,000+ dataset was analyzed with actionable insights and appropriate recommendations generated from it.

### Data Cleaning and Analysis

The required bringing the datasets together using their common features. In the case of power BI, “Merging” is the term used. The various tables were merged using the primary key in each table. The dataset was ‘merged as new’ so as to retain the originality of the dataset.

To define the reviews, a Conditional Column was created to represent Customer Review categories. They include:
- 5 — Very Good
- 4 — Good
- 3 — Medium
- 2 — Fair
- 1 — Poor

A custom column was created to calculate the difference in days from the purchase date and delivery date. 
Average Delivery Time: with column name “Delivery Day(s)” and the result was in hours, minutes, and seconds (hms). So, to achieve the goal of how many days it took to deliver the goods to a customer, the column was converted to Day by highlighting the ‘Delivery Day’ column then from the “Add Column” pane to the “Duration” button another column with the number of days was created which was renamed as the Average Delivery Day(s).
