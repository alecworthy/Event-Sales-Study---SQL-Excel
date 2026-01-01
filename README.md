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

## 📊 Key Insights (Example)

> *(Replace percentages/values with your final numbers once screenshots are locked)*

- Revenue and bookings peak sharply in **November–December**, driven by seasonal Christmas party packages.
- **Seasonal and conference packages** generate the highest average booking value.
- Approximately **X% of customers are repeat buyers**, contributing a disproportionately large share of total revenue.
- The **lead-to-opportunity conversion rate** is approximately **X%**, with an overall **win rate of X%**.
- The average **sales cycle length** is **~X days**, varying by package type and deal size.
- NSW and VIC account for the majority of bookings, but some states show higher average margins.

---

## 📈 Reporting & Outputs

SQL queries generate:
- Monthly KPI tables (bookings, revenue, margin, growth)
- Customer lifetime value proxies
- Funnel conversion and sales cycle metrics
- A **dashboard-ready view** (`vw_daily_salesboard`) suitable for BI tools

Query outputs are exported to Excel for clean, stakeholder-friendly visualisations, which are included in the `/images` folder.

---

## ▶️ How to Run the Project

1. Create a MySQL database (v9.3+)
2. Run scripts in order:
   - `sql/01_schema_mysql.sql`
   - `sql/02_seed_data_mysql.sql`
   - `sql/03_data_quality.sql`
   - `sql/04_kpis.sql`
   - `sql/05_customer_insights.sql`
   - `sql/06_funnel.sql`
   - `sql/07_views.sql`
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
