**Project Title:** Customer Segmentation using RFM (Recency, Frequency, Monetary) Analysis

**Description:**
This project focuses on customer segmentation through RFM analysis to help an e-commerce business better understand its customer base and develop targeted marketing strategies. RFM analysis categorizes customers based on three key behavioral metrics:

* **Recency (R):** How recently a customer made a purchase
* **Frequency (F):** How often a customer makes purchases
* **Monetary (M):** How much money a customer spends

The dataset was sourced from an e-commerce platform and underwent thorough **data cleaning and preprocessing**. This involved removing missing values, eliminating duplicates, correcting data types, and standardizing date formats. From this cleaned data, we extracted meaningful features — including the last purchase date per customer, total purchase count, and total spending — using group-based aggregation.

Using a reference **billing closing date (20th December 2017)**, we calculated the **Recency** value as the number of days since a customer's last transaction. **Frequency** was calculated using invoice counts, and **Monetary** by summing purchase prices. We then computed RFM scores for each customer by dividing each metric into quartiles, where:

* Lower Recency = more valuable,
* Higher Frequency = more valuable,
* Higher Monetary = more valuable.

We assigned each customer a rank (1 to 4) for each of the RFM metrics. The ranks were then summed to generate a **Loyalty Score** ranging from 3 to 12, reflecting overall customer value. Based on this Loyalty Score, customers were classified into four loyalty segments:

* **Platinum:** Highest value customers
* **Gold:** Loyal but with moderate spending or recency
* **Silver:** Occasional buyers
* **Bronze:** Low-value or dormant customers

The final **segmented dataset** included each customer’s ID, Recency, Frequency, Monetary values, and their assigned Loyalty Badge. We visualized the distribution of customers across segments using bar plots, offering clear insights into the customer base composition.

This segmentation enables the business to:

* Identify and reward high-value customers (Platinum)
* Engage moderate-value customers (Gold/Silver) with promotions
* Re-engage or ignore low-value customers (Bronze)
* Personalize marketing campaigns and improve ROI

The final segmented data was exported for further use in targeted campaigns and customer relationship management systems.

**Technologies & Tools Used:**
Python, Pandas, NumPy, Matplotlib, Seaborn, Datetime, Jupyter Notebook
