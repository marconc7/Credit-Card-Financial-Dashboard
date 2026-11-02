# Credit Card Financial & Customer Dashboard

A comprehensive data analytics project designed to deliver real-time operational insights into credit card performance, customer demographics, transaction behaviors, and revenue streams.

---

## 📌 Table of Contents
- [Project Objective](#-project-objective)
- [Dataset & Data Source](#-dataset--data-source)
- [Tech Stack & Architecture](#-tech-stack--architecture)
- [Data Pipeline & Preparation](#-data-pipeline--preparation)
- [Dashboard Reports](#-dashboard-reports)
- [Key Insights (YTD Overview)](#-key-insights-ytd-overview)
- [How to Run This Project](#-how-to-run-this-project)

---

## 🎯 Project Objective

The goal of this project is to develop an interactive, real-time weekly dashboard that monitors credit card operations. It empowers stakeholders to analyze key performance indicators (KPIs) surrounding revenue generation, transaction volumes, interest earnings, and demographic distributions.

---

## 📁 Dataset & Data Source

The project uses two primary data files:
1. `customer_detail.csv`: Customer demographics, income levels, job profiles, and location.
2. `credit_card_detail.csv`: Transaction metrics, revenue generation, card categories, and expenditure types.

> **Source Repository:** [Credit Card Financial Dashboard Data Source](https://github.com/marconc7/Credit-Card-Financial-Dashboard)

---

## 🛠 Tech Stack & Architecture

- **Database Management:** PostgreSQL / SQL Server (SQL table creation & CSV importing)
- **Data Visualization & Analytics:** Power BI Desktop
- **Data Processing:** DAX (Data Analysis Expressions), Power Query
- **Documentation:** Markdown

---

## ⚙️ Data Pipeline & Preparation

1. **Data Acquisition:** Downloaded the raw CSV datasets (`customer` and `credit_card`) from the source repository.
2. **Database Setup:** 
   - Created structured SQL schemas/tables for both datasets.
   - Defined proper primary keys, foreign key relationships, and appropriate data types.
3. **ETL Process:** 
   - Imported CSV records into the SQL database.
   - Performed basic cleaning and data verification steps within SQL.
4. **Power BI Integration:** 
   - Connected Power BI to the SQL database.
   - Configured data models, created relationships between customer and transaction tables, and developed DAX measures for dynamic calculations.

---

## 📊 Dashboard Reports

### 1. Credit Card Customer Report
Focuses on demographic distributions, revenue per customer segment, marital status, income groups, and job types.

### 2. Credit Card Transaction Report
Provides granular visibility into transaction amounts, transaction counts, card category breakdown, payment methods, and expenditure types.

---

## 💡 Key Insights (YTD Overview)

### Financial Summary
- **Overall Revenue:** **$57M**
- **Total Interest Earned:** **$8M**
- **Total Income:** **$588M**
- **Total Transaction Amount:** **$46M**
- **Total Transaction Count:** **667.2K**

### Demographics & Segmentation
- **Gender Contribution:** Male customers generate significantly higher revenue than female customers (**$31M** vs **$26M**).
- **Age Group Breakdown:** Customers in the **40–50 age range** are the primary revenue drivers, accounting for **43.8% of total revenue**.
- **Customer Satisfaction:** Customer Satisfaction Score (CSS) sits at an average of **3.19**.

### Card & Usage Behaviors
- **Card Tier Dominance:** **Blue credit cards** account for **83.5% ($47.2M)** of total revenue.
- **Top Expenditure Category:** Bill payments lead all expenditure types at **$14.0M**, followed by Entertainment (**$9.8M**) and Fuel (**$9.6M**).
- **Preferred Swipe Type:** **Swipe transactions** dominate at **$23M**, followed by Chip (**$17M**) and Online (**$4M**).

---

## 🚀 How to Run This Project

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/marconc7/Credit-Card-Financial-Dashboard.git
   ```

2. **Database Setup:**
   - Execute the SQL table creation script found in `/sql/schema.sql`.
   - Load the `customer.csv` and `credit_card.csv` datasets into their respective tables using your SQL client (e.g., PostgreSQL `\copy` or SQL Server Import Wizard).

3. **Open in Power BI:**
   - Open the `.pbix` file using Power BI Desktop.
   - Update the database credentials/connection string to point to your local database instance if needed.
   - Refresh the data models to view the updated reports.

---

## 📄 License
Distributed under the MIT License. See `LICENSE` for more details.