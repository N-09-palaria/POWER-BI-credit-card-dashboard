# POWER-BI-credit-card-dashboard

 Credit Card Customer Report Dashboard that brings credit card operations to life through data.

💡 Why I built this:
Credit cards aren’t just about transactions — they represent customer journeys, spending habits, and lifestyle preferences. My goal was to design a dashboard that doesn’t just display numbers, but helps stakeholders see the story behind the data.

📊 How I built it:

⚙️ Step 1: Import Data to PostgreSQL Database

Prepare CSV File – Clean and structure the dataset.

Create Tables in SQL – Define schema for storing credit card details.

Import CSV into SQL – Used COPY command to load CSV data into the database.

Added 53 weeks of data into the existing table to keep the dashboard automated and up to date.

🛠 Step 2: Data Processing & Transformation

Performed preprocessing in PostgreSQL.

Handled date formatting for week_start_date.

Applied business rules for revenue, income, and customer segmentation.

📊 Step 3: DAX Queries in Power BI

Key measures created for analysis:
week_num2 = WEEKNUM('public cc_detail'[week_start_date])
Revenue = 'public cc_detail'[annual_fees] + 'public cc_detail'[total_trans_amt] + 'public cc_detail'[interest_earned]

Used SWITCH function for categorization:

Income Groups (High, Medium, Low)
Age Groups
Card Categories (Gold, Silver, Blue, Platinum)

🌟 What the dashboard shows:

40–50 age group, high-income professionals, and graduates contribute the highest revenue.

Swipe and online transactions lead in usage compared to chip-based payments.

Texas, New York, and California stand out as top-performing states.

🚀 Tech Stack

Database: PostgreSQL

Visualization Tool: Power BI

Languages: SQL, DAX

Data Source: CSV files

📷 Dashboard Snapshot

Screenshot 2025-09-20 204807.png

💡 Key Learning

This project was not just about building visuals but about end-to-end data handling:

From data import → SQL processing → DAX calculations → insightful dashboards.

Learned how to automate reporting by continuously feeding new data into PostgreSQL.

🙌 Feedback & Collaboration

I’d love your feedback on this project. Feel free to fork, raise issues, or share suggestions!
