---
# 🛍️ Data Analytics Project — Shopping Analysis of a Customer
---

## 📘 Project Overview

This project simulates a real-world **retail analytics scenario**, analyzing how customers shop, what drives their purchases, and how discount, demographics, and subscription behavior affect sales.  

It demonstrates an **end-to-end data analytics workflow** — from **data cleaning (Python)** and **data modeling (SQL)** to **visualization and storytelling (Power BI)**.

> 🧾 Note: The dataset is **synthetic** and generated for educational and business simulation purposes.

---

## 🧩 Project Structure
- **Data Preparation (Python)** – Cleaned and preprocessed raw sales data using pandas & NumPy.  
- **Database Modeling (PostgreSQL)** – Structured the dataset into relational tables.  
- **Exploratory Data Analysis (SQL)** – Performed queries to uncover customer insights and behavioral patterns.  
- **Dashboard Visualization (Power BI)** – Designed an interactive report highlighting performance metrics and KPIs.  
- **Report & Presentation** – Summarized findings in professional documentation and slides.  

---

## 🛠️ Tools & Technologies
| Tool / Technology | Purpose |
|-------------------|----------|
| **Python (pandas, NumPy)** | Data cleaning and preprocessing |
| **PostgreSQL / SQLAlchemy** | Data storage, querying, and modeling |
| **Power BI** | Visualization, dashboards, and storytelling |
| **Excel** | Data validation and tabular exports |
| **Git & GitHub** | Version control and sharing |

---

## 🧱 Dataset Summary
| Feature | Description |
|----------|--------------|
| **Records** | ~3,900 |
| **Columns** | 18 |
| **Data Types** | Customer, Transaction, and Behavioral Metrics |
| **Missing Values** | 37 missing ratings handled with median imputation |
| **Source** | Synthetic dataset for analytics learning |

Key fields include:  
`customer_id`, `age`, `gender`, `location`, `subscription_status`, `product_name`, `category`, `purchase_amount`, `review_rating`, `shipping_type`, `discount_applied`.

---

## 📊 Business Problems Solved
1. Identify **top-spending customers** and their demographic trends.  
2. Evaluate **impact of discounts** on high-value buyers.  
3. Discover **top-rated products** by customer satisfaction.  
4. Compare **purchase behavior across shipping types**.  
5. Analyze **subscriber vs non-subscriber revenue contribution**.  
6. Identify **most discounted and profitable products**.  
7. Segment customers into **New, Returning, and Loyal**.  
8. Measure **repeat purchase correlation** with subscription status.  
9. Track **revenue contribution by age group**.  
10. Recommend strategies to increase **retention and loyalty**.

---

## 💻 Sample SQL Queries

```sql
-- 🧾 Total Revenue by Gender
SELECT gender, SUM(purchase_amount) AS total_revenue
FROM customers
JOIN orders USING(customer_id)
GROUP BY gender
ORDER BY total_revenue DESC;

-- 🛒 Top 5 Products by Review Rating
SELECT product_name, ROUND(AVG(review_rating), 2) AS avg_rating
FROM orders
GROUP BY product_name
ORDER BY avg_rating DESC
LIMIT 5;
```

---

##🖼️ Visual Insights
🧮 Table Overview
<p align="center"> <img src="Tables.jpg" alt="Data Model Tables" width="80%"> </p>
📊 Power BI Dashboards

The DASHBOARD folder contains 4 interactive visual snapshots that illustrate:
Revenue Breakdown (by Gender, Age, Region)
Discount Impact vs Spending
Customer Segmentation (Loyal, New, Returning)
Top Products & Shipping Insights

<p align="center"> <img src="DASHBOARD/Home.jpg" alt="Dashboard 1" width="45%"> <img src="DASHBOARD/PAGE_1.jpg" alt="Dashboard 2" width="45%"> </p> <p align="center"> <img src="DASHBOARD/PAGE_2.jpg" alt="Dashboard 3" width="45%"> <img src="DASHBOARD/PAGE_4.jpg" alt="Dashboard 4" width="45%"> </p>

---

##🧠 Key Learnings

Enhanced ability to integrate Python, SQL, and Power BI in a single analytics workflow.

Improved understanding of customer segmentation and behavioral metrics.

Developed skills in data cleaning, visualization, and storytelling.

Gained practical experience in end-to-end retail analytics.

---

##📄 Documentation

Detailed reports and presentations are included for deeper insights:

File	Description
📘 REPORT – Shopping Analysis of Customers.pdf
	Full report including SQL, Python, and Power BI insights
📊 PPT – Shopping Analysis Presentation.pptx
	Business presentation with dashboards and findings
🧾 Regional_Sales_Analysis.ipynb
	Jupyter Notebook for Python data cleaning and transformation
📈 Sales Analysis Dashboard.pbix
	Power BI dashboard file
📊 Sales_data(EDA Exported).csv
	Cleaned dataset exported for BI tools

These materials provide a complete view of the analytics process from raw data to decision-ready insights.

---

##🧾 Conclusion

This project demonstrates how a data analyst can leverage Python, SQL, and Power BI to transform raw retail data into actionable business intelligence.
It showcases data storytelling, analytical thinking, and dashboarding — essential skills for a Data Analyst / BI Developer.

---

##⚠️ Disclaimer

All datasets and results are AI-generated and purely educational.
This project is intended for learning and portfolio demonstration purposes.

---

##👨‍💻 Author

Mukesh Gopi Nandh
📧 mukeshudatha7@gmail.com

🌐 Connect with Me:

<p align="left"> <a href="https://github.com/Mukeshgn" target="_blank"> <img src="https://img.shields.io/badge/GitHub-Mukeshgn-181717?style=for-the-badge&logo=github" alt="GitHub"/> </a> <a href="https://www.linkedin.com/in/mukesh-gopi-nandh" target="_blank"> <img src="https://img.shields.io/badge/LinkedIn-Mukesh%20Gopi%20Nandh-blue?style=for-the-badge&logo=linkedin" alt="LinkedIn"/> </a> </p>
