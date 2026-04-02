# Curtomer_churn_prediction_DA
About Dataset
Brazilian E-Commerce Public Dataset by Olist
Welcome! This is a Brazilian ecommerce public dataset of orders made at  Olist
Store . The dataset has information of 100k orders from 2016 to 2018 made at
multiple marketplaces in Brazil. Its features allows viewing an order from multiple
dimensions: from order status, price, payment and freight performance to
customer location, product attributes and finally reviews written by customers. We
also released a geolocation dataset that relates Brazilian zip codes to lat/lng
coordinates.
This is real commercial data, it has been anonymised, and references to the
companies and partners in the review text have been replaced with the names of
Game of Thrones great houses.

Classified Dataset
We had previously released a classified dataset, but we removed it at Version 6.
We intend to release it again as a new dataset with a new data schema. While we
don&#39;t finish it, you may use the classified dataset available at the Version 5 or
previous.
Inspiration
Here are some inspiration for possible outcomes from this dataset.
NLP:
This dataset offers a supreme environment to parse out the reviews text through
its multiple dimensions.
Clustering:
Some customers didn&#39;t write a review. But why are they happy or mad?
Sales Prediction:
With purchase date information you&#39;ll be able to predict future sales.
Delivery Performance:
You will also be able to work through delivery performance and find ways to
optimize delivery times.
Product Quality:
Enjoy yourself discovering the products categories that are more prone to
customer in satisfaction.

CLIENTS REQUIREMENTS & WE HAVE TO DO

Sales Trend Analysis (Easy)
Client requirement:
“Our monthly sales are fluctuating. Can you analyze the sales data and tell us how revenue has changed month by month?”
Student Task:
Convert date to month
Group by month → sum revenue
Plot a simple line chart
Give a 3-line business insight
Top Customers Identification (Easy)
Client requirement:
“We want to identify our top spending customers. Can you give the list of top 10 customers based on total amount spent?”
Student Task:
Group by customer_id
Aggregate total purchase amount
Rank and list top 10
Missing Data Problem (Easy)
Client requirement:
“There are missing values in the product weight column. Tell us how many are missing and fill them with a reasonable approach.”
Student Task:
Check missing count
Fill with mean/median
Explain in 1–2 lines why they chose that method
Customer Recency Analysis (Medium)
Client requirement:
“We want to understand when customers made their last purchase. Can you calculate a recency column for each customer?”
Student Task:
Convert dates
For each customer, take max(order_date)
Subtract from max overall date
Create recency_days
Product Category Performance (Medium)
Client requirement:
“Which product categories are performing well? Give us total sales and number of orders for each category.”
Student Task:
Merge orders + order_items + product table
Group by product_category
Compute total revenue & total orders
Sort descending

Repeat Customer Rate (Medium)
Client requirement:
“What percentage of customers made more than one purchase?”
Student Task:
Group customers
Count their orders
Calculate % with order_count > 1
Shipping Delay Analysis (Medium)

Client requirement:
“Our customers are complaining about delivery delays. Can you tell us what percentage of orders were delivered late?”
Student Task:
Compare actual vs estimated delivery date
Create delay_flag
Calculate % delayed
Payment Method Usage (Easy/Medium)
Client requirement:
“We want to know which payment method is most popular. Can you give the count of orders per payment_type?”
Student Task:
Use payments table
Group by payment_type
Count number of orders
Correlation Check Between Price & Review Score (Medium)
Client requirement:
“We want to check if expensive products get better reviews. Can you check the correlation between product price and review score?”
Student Task:
Merge order_items + reviews
Group or take average
Compute correlation using .corr()
Write 3 lines of interpretation
Simple Customer Segmentation (Medium)
Client requirement:
“We want to group customers based on their total spend into: Low, Medium, High value segments.”
Student Task:
Aggregate total_spend for each customer
Use pd.qcut() or manual rules
Create segment column
Give insights (e.g., how many in each segment)
Feature Engineering:
Create features from this rich dataset or attach some external public information
to it.
