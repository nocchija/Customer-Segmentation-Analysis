# Customer-Segmentation-Analysis
Customer segmentation and CRM analysis using Python.

## Project Overview
This project analyses e-commerce transactional data to understand customer purchasing behaviour and identify meaningful customer segments.

The objective is to translate customer data into actionable CRM and marketing strategies.

## Business Objectives / Questions
1. Who are the company's most valuable customers?
2. Which customers are at risk of churn?
3. How can different customer segments be targeted different?

The objective of this project is to **analyse customer purchasing behaviour** and **identify meaningful customer segments that can support more targeted and effective marketing strategies.******

This analysis aims to:
- Identify the company's most valuable customer segments.
- Identify customers who may be at risk of churn or disengagement.
- Identify opportunities for customer reactivation and retention.
- Understand differences in purchasing behaviour across customer segments.
- Develop actionable CRM and marketing recommendations for each segment.

## Dataset
The project uses the UCI Online Retail dataset, which contains transactional data from a UK-based online retailer between December 2010 and December 2011.

The dataset includes information such as:
- Invoice number
- Product
- Quantity
- Transaction date
- Unit price
- Customer ID
- Customer country

## Tools Used

- Python
- Pandas
- Jupyter Notebook
- VS Code

## Data Cleaning
The dataset was cleaned before analysis to ensure that customer purchasing behaviour was represented appropriately. This included:

- Removing transactions without a Customer ID.
- Removing cancelled or returned transactions with negative quantities.
- Removing transactions with zero or negative unit prices.
- Removing exact duplicate rows.
- Converting transaction dates into a suitable date format.

The final cleaned dataset contains 392,692 transaction records.

## Data Analysis
Exploratory analysis was conducted to understand overall customer and purchasing behaviour before customer segmentation.

Key findings include:

- 4,338 unique customers generated approximately £8.89 million in revenue.
- The United Kingdom contributed approximately 81.97% of total revenue.
- Between August and November 2011, order volume increased by approximately 108%, while revenue increased by approximately 80%.
- Average order value decreased by approximately 14% over the same period, suggesting that the revenue increase was primarily driven by higher order volume rather than larger orders.

December 2011 was excluded from month-on-month trend interpretation as the dataset only contains transactions up to 9 December.

## RFM Customer Segmentation

Customers were segmented using RFM analysis:

- **Recenc (R):** How recently the customer made a purchase.
- **Frequency (F):** How frequently the customer placed orders.
- **Monetary (M):** How much the customer spent.

Customers were grouped into five CRM segments:

- High-Value Loyal
- Regular
- Recent / Low Frequency
- Risk of Churn (RoC)
- Inactive / Low Frequency

## Key Findings

- **High-Value Loyal customers** represent 18.19% of customers but contribute 61.26% of total revenue, making retention of this segment a key priority.
- **Regular customers** form the largest segment at 36.72% of customers and contribute 23.55% of revenue, presenting an opportunity to grow customer value.
- **Inactive / Low Frequency customers** represent 30.77% of customers but only 7.67% of revenue, suggesting that expensive blanket reactivation campaigns may not be cost-effective.
- Within the **Risk of Churn** segment, the 10 highest-spending customers account for 27.58% of the segment's historical revenue, suggesting that win-back efforts could be prioritised based on historical customer value.

## Recommendations
Based on the earlier findings, I also made marketing recommendations for each customer segment, mainly prioritising the High-Value Loyal customers and Regular customers.

## Limitations

- The dataset covers a limited historical period and therefore does not represent current customer behaviour.
- Customer segments are inferred from transactional behaviour and do not confirm whether a customer has actually churned.
- Imperfect information: The dataset does not contain marketing campaign exposure or engagement data, so the proposed CRM strategies and A/B test are recommendations rather than measured campaign results.