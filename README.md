

🏙️ Luxury Housing Sales Analysis – Bengaluru

An end-to-end data analytics & BI project analyzing luxury housing transactions in Bengaluru using Python, SQL Server, and Power BI.
The project focuses on booking behavior, pricing trends, builder performance, and market insights.

📌 Project Overview

This project analyzes luxury housing sales data to answer key business questions such as:

Which builders dominate revenue and bookings?

How do bookings change quarter-by-quarter?

Which micro-markets and configurations perform best?

How do amenities and sales channels impact booking conversion?

The pipeline follows a real-world analytics workflow:
CSV → Python cleaning → SQL Server → Power BI dashboards

🛠️ Tech Stack
Layer	Tools
Data Cleaning & Feature Engineering	Python (Pandas, NumPy)
Database	SQL Server
BI & Visualization	Power BI (DirectQuery, DAX)
Version Control	Git & GitHub
📂 Dataset Description

The dataset contains luxury housing transactions with the following key fields:

Property_ID

Project_Name

Developer_Name

Micro_Market

Configuration

Ticket_Price_Cr

Unit_Size_Sqft

Transaction_Type

Purchase_Quarter

Amenity_Score

Sales_Channel

Possession_Status

Buyer_Type

NRI_Buyer

🧹 Step 1: Python — Data Cleaning & Feature Engineering
✔ Data Cleaning

Standardized inconsistent price formats (₹, Cr, commas)

Handled missing values using median-based imputation

Normalized text fields to avoid duplicate categories

✔ Feature Engineering

Derived analytical columns:

Price_per_Sqft

Booking_Flag (Primary vs Resale)

Quarter_Number

Year

Quarter Label (Q1–Q4)

Output: DB-ready cleaned dataset

🗄️ Step 2: SQL Server — Data Storage & Validation
✔ Database Design

Optimized schema with correct data types (BIT, TINYINT, FLOAT)

Boolean flags stored using BIT for data integrity

✔ Validation Queries

Record counts

Booking distribution

Revenue & average ticket size per builder

Micro-market conversion analysis

📊 Step 3: Power BI — Interactive Dashboard
✔ DirectQuery Connection

Live connection to SQL Server (house2.dbo.house_data_3)

✔ Key DAX Measures

Total Bookings

Total Transactions

Booking Conversion %

Total Revenue

Average Ticket Size

Project Count

📈 Dashboard Insights
Market Trends

Quarterly booking trends across micro-markets

Builder Performance

Top builders by revenue and average ticket size

Booking Conversion

Conversion rates by micro-market and sales channel

Amenity Impact

Relationship between amenity score and booking success

Configuration Demand

Most in-demand housing configurations (2BHK, 3BHK, etc.)

Geographical Insights

Concentration of luxury projects across Bengaluru

🎯 Key Business Insights

Premium builders consistently dominate both revenue and booking volume

Certain micro-markets show high conversion despite fewer listings

Amenity score positively correlates with booking success

Digital and broker-assisted channels outperform others in conversions

📌 Project Structure
├── data/
│   ├── raw_housing_data.csv
│   ├── cleaned_housing_data.csv
│
├── notebooks/
│   ├── data_cleaning_feature_engineering.ipynb
│
├── sql/
│   ├── table_creation.sql
│   ├── validation_queries.sql
│
├── powerbi/
│   ├── Luxury_Housing_Dashboard.pbix
│
├── README.md

🚀 How to Run This Project

Clean the CSV using Python

Load cleaned data into SQL Server

Connect Power BI using DirectQuery

Build visuals using provided DAX measures

🎤 Interview Talking Point

“This project demonstrates a complete analytics workflow — from raw data cleaning and feature engineering to SQL modeling and interactive Power BI dashboards with business-driven insights.”

🔮 Future Enhancements

Add a proper Date Dimension table

Builder-level performance ranking using RANKX

Predictive booking probability model

Deployment using Power BI Service

📬 Contact

Author: [Your Name]
📧 Email: [your.email@example.com
]
🔗 LinkedIn: [your LinkedIn profile]
