# Customer Behavior and Sales Pattern Analysis in the Snack Industry

## Project Overview

This data analytics project investigates customer segmentation, purchasing behavior, and sales patterns for a leading chip retailer. The analysis explores various dimensions including customer lifestyle stages, customer types (mainstream, premium, budget), product preferences by size and brand, and seasonal trends. Feature engineering and statistical hypothesis testing were employed to generate actionable insights for improving inventory planning, targeted marketing, and promotional strategies.

## Dataset Description

The analysis uses two primary datasets:

- **Customer Data**: Customer segmentation by life stage (LIFESTAGE) and spending behavior (CUSTOMER_TYPE); ~ 72,000+ records.

- **Transaction Data**: Purchase transactions including product names, quantities, prices, and dates; ~ 2,60,000+ records.

Key points:

- Data spans an entire calendar year.

- Transaction dates required transformation from Excel integer format to datetime.

- Product names contained embedded weight information (e.g., "250g") requiring feature engineering.

## Project Structure
The workflow follows a structured analytics pipeline:

1) Data Preparation
   - Cleaned and feature engineered product names.

   - Fixed transaction date fields.

   - Updated column names for better clarity.

2) Feature Engineering
   - Extracted packet size (grams) from product names.

   - Calculated total sales per transaction and spend per customer.

   - Aggregated sales data across brands, packet sizes, and customer groups.

3) Exploratory Data Analysis (EDA)
   - Examined customer demographic distributions.

   - Analyzed sales performance by brand and product size.

   - Identified seasonal patterns in sales volume.

4) Statistical Analysis
   - Conducted independent two-sample t-tests to assess spending behavior differences between customer groups.

   - Verified significance of observed behavioral patterns.

5) Insights and Strategic Recommendations
   - Synthesized findings into actionable strategies for inventory and marketing optimization.

## Features Used
Original Dataset Columns:

1) Customer Dataset: `LYLTY_CARD_NBR`, `LIFESTAGE`, `PREMIUM_CUSTOMER`
   
2) Transaction Dataset: `DATE`, `STORE_NBR`, `LYLTY_CARD_NBR`, `TXN_ID`, `PROD_NBR`, `PROD_NAME`, `PROD_QTY`, `TOT_SALES`

Feature Engineered Columns:
- `PROD_BRAND`
- `PROD_SIZE`
- `UNIT_PRC`

## Key Insights
- Kettle was the top-selling brand throughout the year.

- 175g packet size dominated sales across all customer segments.

- Budget older families and mainstream young singles/couples were the primary contributors to overall sales.

- Seasonal spikes, particularly around Christmas, suggest strong promotional opportunities.

- Younger mainstream customers demonstrated higher spend-per-transaction, indicating potential for upselling and impulse buying strategies.

## Recommendations
- Focus inventory and promotional efforts around Kettle products and 175g packet sizes.

- Implement segment-specific marketing to target high-value customer groups.

- Scale marketing campaigns and stock replenishment 2–3 weeks before Christmas to capitalize on peak demand.

- Position complementary products strategically to appeal to impulse buying tendencies observed in younger customer segments.

## Tools and Technologies
![](https://img.shields.io/badge/Python-3776AB.svg?style=for-the-badge&logo=Python&logoColor=white)
![](https://img.shields.io/badge/Jupyter-F37626.svg?style=for-the-badge&logo=Jupyter&logoColor=white)
![](https://img.shields.io/badge/pandas-150458.svg?style=for-the-badge&logo=pandas&logoColor=white)
![](https://img.shields.io/badge/NumPy-013243.svg?style=for-the-badge&logo=NumPy&logoColor=white)
![](https://img.shields.io/badge/SciPy-8CAAE6.svg?style=for-the-badge&logo=SciPy&logoColor=white)
![](https://img.shields.io/badge/Matplotlib-%23ffffff.svg?style=for-the-badge&logo=Matplotlib&logoColor=black)

## Sample Visuals
![image](https://github.com/user-attachments/assets/faabd0b5-5e75-4284-a091-47c0a0abc575)
![image](https://github.com/user-attachments/assets/3a5d3c84-0b46-4785-ae17-9ec37a32d570)
![image](https://github.com/user-attachments/assets/ecc3e23d-5b9b-4cf4-b419-e2a37722726d)
![image](https://github.com/user-attachments/assets/1a6cb6b7-8a9e-42b5-9e48-11635c90b292)
![image](https://github.com/user-attachments/assets/09c95562-2c4d-4f94-8cac-d06eaa87fcfc)
![image](https://github.com/user-attachments/assets/c2080c7b-9dec-4023-82b7-4abdf1bec0b2)
![image](https://github.com/user-attachments/assets/8873d5b3-c50f-4d21-8832-23f73ee7f98e)
![image](https://github.com/user-attachments/assets/18715990-c8c1-45cb-882b-2739ed936d8a)
![image](https://github.com/user-attachments/assets/847786e6-06c0-4ed8-bf02-1ee532c3e307)
![image](https://github.com/user-attachments/assets/7b0b9d28-d0f8-4bf1-be19-3e9578c93cbd)
![image](https://github.com/user-attachments/assets/f3496e55-fe8a-4970-9417-ccb9af528247)
![image](https://github.com/user-attachments/assets/a189ad7a-23ad-4d0e-a644-49abd29addbc)
![image](https://github.com/user-attachments/assets/94bfe487-4187-458f-84af-cfa3288abc78)

## Quick Summary
This project showcases how thoughtful data cleaning, feature engineering, and statistical validation can uncover valuable insights hidden within retail transaction data — and how those insights can directly translate into better business decisions.

