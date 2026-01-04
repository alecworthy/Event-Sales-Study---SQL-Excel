# Australian Events Sales Performance & Customer Insights (SQL)

## 📌 Project Overview

This project analyses sales performance and customer behaviour for a simulated **Australian events company** offering corporate event packages (e.g. team building, conferences, Christmas parties).

Using **MySQL Community Server 9.3**, I designed a realistic CRM-style data model and wrote SQL queries to evaluate revenue trends, sales funnel performance, and customer value. The project demonstrates end-to-end analytics work — from data modelling and validation through to KPI reporting and insight generation.

---

## 🎯 Business Questions

This analysis answers key commercial questions, including:

- How is **revenue and booking volume trending over time**?
- Which **event packages** drive the most revenue and margin?
- What does the **sales funnel** look like from lead → opportunity → win?
- How long does the **sales cycle** take on average?
- What proportion of revenue comes from **repeat customers**?
- How does performance vary by **state, customer segment, and sales team**?

---

## 🛠️ Tools & Technologies

- **MySQL Community Server 9.3**
- **MySQL Workbench**
- SQL (CTEs, window functions, aggregations)
- Excel (for visualisation of query outputs)

---

## 🗂️ Data Model

The database simulates a real-world CRM and sales environment with the following core tables:

- `customers` – company details, industry, state
- `leads` – inbound enquiries and lead sources
- `opportunities` – sales pipeline stages and deal values
- `bookings` – confirmed events with revenue and cost
- `packages` – event package catalogue
- `sales_reps` – sales ownership
- `payments` – deposits and balances

The dataset contains **1,000 confirmed bookings** across 2024–2025, with a realistic **Nov–Dec seasonal spike** reflecting Christmas party demand.

---

## ✅ Data Quality & Validation

Before analysis, a series of data quality checks were performed to ensure reliability, including:

- Duplicate customer detection  
- Orphan record checks (leads, opportunities, bookings)  
- Revenue and cost sanity checks  
- Margin validation (revenue vs cost)  
- Payment reconciliation (payments exceeding revenue)  
- Stage completeness checks (won/lost deals with missing close dates)

These checks help ensure that reported insights are trustworthy and business-ready.

---

## 📊 Key Insights

- Revenue and bookings peak sharply in **November–December**, driven by seasonal Christmas party packages.
- **Retreat and Launch** generate the highest average booking value.
- The biggest percentage growth was **135%** that happending from November to December.  
- The top customers have an average of **9** repeat bookings. 
- SA and VIC account for the majority of bookings, but some states show higher average margins.

---

## 📈 Reporting & Outputs

SQL queries generate:
- Monthly KPI tables (bookings, revenue, margin, growth)
- Customer lifetime value proxies
- Funnel conversion and sales cycle metrics
- A **dashboard-ready view** (`vw_daily_salesboard`) suitable for BI tools

Query outputs are exported to Excel for clean, stakeholder-friendly visualisations.

---

## 📊 Screen Shots & Visualisations


Monthly Sale KPIs: Pulled from Excel showing the comparison between Revenue, Costs and Margin over 2 years. 

<img width="737" height="352" alt="image" src="https://github.com/user-attachments/assets/56dabdd9-4caa-4209-adcf-640f137aaf1e" />

Percentage Revenue Growth: Pulled from Excel showing the percentage reveue increase and decrease across the 2 years. 

<img width="746" height="400" alt="image" src="https://github.com/user-attachments/assets/76bf07fd-bcbc-41c9-acec-c7e02164badf" />

Christmas Spike: Pulled from Excel showing the increase of sales over the Christmas period and leading into the New Year. 

<img width="541" height="322" alt="image" src="https://github.com/user-attachments/assets/5e990dd3-9f87-434f-95a4-093ea7208406" />

State Performance: Pulled from MySQL showing the State Performance sales.

<img width="1322" height="577" alt="image" src="https://github.com/user-attachments/assets/f2010d95-6920-4674-b6f3-47b91fa0ef0f" />

Top Customers: Pulled from Excel showing the top 10 Customers with the highest Sales. 

<img width="403" height="266" alt="image" src="https://github.com/user-attachments/assets/5409d1c9-818d-4510-9205-0b9ae9d74963" />

---

## ▶️ How to Run the Project

1. Create a MySQL database (v9.3+)
2. Run scripts in order: [See code here](https://github.com/alecworthy/Event-Sales-Study---SQL-Excel/blob/main/SQL%20Full%20code)
3. Export result sets as CSV for visualisation in Excel

---

## 🔒 Data Disclaimer

All data in this project is **synthetic and anonymised**.  
The structure and analysis reflect real-world event sales scenarios, but no commercial or customer data is used.

---

## 🚀 Portfolio Context

This project forms part of my broader data analytics portfolio, demonstrating:

- Practical SQL proficiency
- Business-focused KPI design
- Data quality awareness
- Customer and revenue analytics
- Clear communication of insights
