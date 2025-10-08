

# 💳 Credit Card Transaction Analysis & Insights (PostgreSQL + Power BI)

## 📊 Project Overview

This project explores credit card transaction data to uncover insights about customer spending behavior, revenue generation, and card performance.
The goal was to design a **complete analytics workflow** — from **raw data ingestion (CSV)** to **database structuring (PostgreSQL)** and **interactive reporting (Power BI)** — similar to how analytics teams manage real financial data.

---

## 🎯 Project Objective

To analyze credit card transactions and understand:

* Revenue and interest trends
* Card category performance (Gold, Silver, Blue, Platinum)
* Customer spending by income group, education, and occupation
* Channel usage (Swipe, Chip, Online)
* Quarterly and weekly transaction insights

---

## 🧩 Tools & Technologies

| Tool            | Purpose                                                |
| --------------- | ------------------------------------------------------ |
| **PostgreSQL**  | Database creation, structured data storage, and import |
| **Power BI**    | Interactive dashboarding and DAX-based KPI computation |
| **Excel / CSV** | Raw data preparation                                   |

---

## ⚙️ Data Workflow

### 🪣 Step 1: Data Sourcing / Ingestion

I started with **raw CSV files** — my foundation for building this analytical “house.”
Using **PostgreSQL**, I:

* Created structured tables using simple SQL commands like `CREATE TABLE`.
* Loaded data efficiently using the `\COPY` command.
* Ensured all files were stored and related consistently.

> 🧠 **Key Learning:** Even simple commands can create a powerful data backbone when structured correctly.

---

### 🧹 Step 2: Data Cleaning & Transformation

Within the PostgreSQL environment, I focused on **data accuracy and reliability**:

* Verified column data types (e.g., `DATE`, `NUMERIC`, `VARCHAR`).
* Fixed date formatting issues (converted `DD-MM-YYYY` → `YYYY-MM-DD`).
* Checked data consistency before visualization.
* Appended **Week 53 data** into the main transaction table to automate continuous reporting.

> ⚙️ SQL Focus: Table creation, data import using COPY, column validation, and basic transformations.

---

### 🧠 Step 3: Dashboard Development in Power BI

After ensuring clean and structured data, I connected PostgreSQL to Power BI to bring the story to life:

* Designed **DAX measures** for total revenue, total interest, transaction count, and card category performance.
* Used **slicers and filters** for dynamic interaction (by Gender, Quarter, Card Type, and Income Level).
* Built a consistent **data model** to ensure accurate drill-down and filtering.
* Refreshed the dashboard automatically after appending new week data.

---

## 📈 Key Insights

* 💰 **Blue Card** category generated the highest revenue (₹47M+).
* 📆 **Q4** saw the highest transaction count and revenue growth.
* 🧑‍🎓 **Graduates and businessmen** drove the majority of card usage.
* 🛍️ **Bills, fuel, and entertainment** were the top spending categories.
* 💳 **Swipe mode** dominated, indicating higher in-person transaction preference.

---

## 🧩 Learnings

* Practiced **end-to-end BI workflow** from raw CSV to dashboard.
* Improved database skills through **PostgreSQL table management and import automation**.
* Understood the importance of **data validation before visualization**.
* Enhanced Power BI storytelling with DAX and dynamic visuals.

---

## 🚀 Future Scope

* Add Python or Power Automate layer for predictive analysis & scheduled refresh.
* Integrate additional demographic datasets for deeper segmentation.
* Introduce benchmarking visuals for comparing customer categories.

---
## 📸 Dashboard Preview

### 1️⃣ Credit Card Weekly Performance Dashboard
![Credit Card Dashboard](dashboard/Dashboard_Screenshots/credit_card_overview.png)

### 2️⃣ Customer Segment & Spending Insights
![Customer Insights](https://github.com/N-09-palaria/POWER-BI-credit-card-dashboard/blob/main/Screenshot%202025-09-20%20204807.png)


## 📂 Repository Structure

```
📁 Credit-Card-Transaction-Analysis
│
├── data/
│   ├── credit_card_transactions.csv
│   ├── customers.csv
│
├── sql/
│   ├── table_creation.sql
│   ├── copy_import_command.sql
│
├── dashboard/
│   ├── Credit_Card_Transaction_Report.pbix
│   ├── Dashboard_Screenshots/
│
├── README.md
```

---

## 👩‍💻 About Me

**Nikita Palaria**
MBA (Finance & Business Analytics) | Data & Business Analytics Enthusiast

📊 Skilled in Power BI, Tableau, Excel, and SQL
💡 Passionate about building meaningful insights from real-world data
📍 Greater Noida 

**Connect:**
🔗 [LinkedIn](https://linkedin.com/in/nikita-palaria)
💻 [GitHub](https://github.com/NikitaPalaria)

---

⭐ *If you found this project insightful, don’t forget to star the repo!*

