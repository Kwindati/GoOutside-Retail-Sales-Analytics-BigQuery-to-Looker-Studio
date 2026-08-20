# GoOutside Retail & Sales Analytics

**End-to-end data analytics project using BigQuery, SQL and Looker Studio**

## Project Overview

GoOutside is a growing adventure and camping gear supplier with a rapidly expanding product portfolio and customer base. The company had several years of sales and product information stored across disconnected CSV files, making it difficult for different teams to access, analyze and use the data for decision-making.

The objective of this project was to transform the available raw business data into a structured analytics solution that could support management decisions around **retail markets, sales performance and order methods**.

I developed an end-to-end analytics workflow using **Google BigQuery, SQL and Looker Studio (formerly Google Data Studio)** to organize the data, perform business analysis and communicate the results through interactive dashboards.

---

## Business Questions

The analysis focused on two main business areas.

### 1. Retail Market Analysis

The Head of Retail Partnerships wanted to understand the structure of the markets in which GoOutside operates.

Key questions included:

* Which retailers contribute the largest share of sales?
* Are individual markets dominated by a small number of large retailers?
* Which markets are more fragmented and competitive?
* Where should GoOutside focus on increasing sales per retailer?
* Where would increasing the number of active retailers potentially create more market activity?

For markets dominated by larger retailers, the business objective was to explore the potential impact of increasing sales volume per retailer by **10%**.

For more competitive markets, the objective was to consider the potential impact of increasing the number of retailers by **15%**.

---

### 2. Order Method Analysis

The Finance Manager wanted to understand whether all available order methods provide sufficient value relative to the resources required to operate them.

The analysis therefore examined:

* Number of orders by order method
* Total sales by order method
* Contribution of different order methods
* Relative performance of order methods
* Potential low-performing order methods that may require further investigation

The goal was to provide a data-driven basis for decisions regarding the future of different order channels.

---
## Dashboard Interactive Preview

The final analysis was presented through an interactive Looker Studio dashboard designed
to provide stakeholders with an accessible overview of sales performance, market
composition and order-method performance. Open the **folder** **Looker Studio Dashboard photos** for easy access or click the **link below** for interactive dashboard:

[View the Interactive Looker Studio Dashboard][https://datastudio.google.com/reporting/cadd642f-ea43-401f-ab55-7218611a32a4]

## Data Availability

### Note on BigQuery Data Availability

The data for this project was stored and analyzed using Google BigQuery, where the SQL queries and analytical transformations were developed as part of the project workflow.

The project was completed using the BigQuery Sandbox/free-tier environment, in which tables created in the sandbox are subject to a limited retention period and may expire after 60 days. As a result, the original BigQuery dataset and associated query environment are no longer available for direct access.

The underlying GoOutside case-study dataset is publicly available, and the SQL logic and analytical workflow developed during the project are documented in this repository. This allows the analysis to be reviewed and, where appropriate, reproduced using the publicly available source data.

### SQL Queries

The SQL queries used for data exploration, transformation and analysis were developed directly in BigQuery. Since the original BigQuery environment is no longer accessible due to the Sandbox retention period, the relevant SQL queries are provided in this repository for transparency and reproducibility.

---
# Data Analytics Workflow

The project followed an end-to-end data analytics workflow:

```text
Raw CSV Data
     ↓
Data Preparation
     ↓
Google BigQuery
     ↓
SQL Queries & Data Analysis
     ↓
Analytical Results
     ↓
Looker Studio / Google Data Studio
     ↓
Interactive Business Dashboard
     ↓
Business Insights & Recommendations
```

---

# Technology Stack

### Data Storage & Processing

* **Google BigQuery**
* SQL
* Google Sheets

### Data Analysis

* SQL
* Business KPI analysis
* Aggregation and segmentation
* Market composition analysis
* Order method performance analysis

### Data Visualization

* **Looker Studio / Google Data Studio**
* Interactive dashboards
* KPI reporting
* Charts and tables

---

# Data Warehouse

The raw CSV data was organized and stored in **Google BigQuery**, providing a structured and scalable environment for querying and analysis.

BigQuery was used as the central analytical data layer rather than performing the analysis directly on disconnected CSV files.

This allowed the data to be queried efficiently and provided a consistent source for the downstream reporting and visualization layer.

---

# SQL Analysis

SQL was used to transform the stored data into business-relevant analytical datasets.

The analysis included:

* Sales aggregation
* Order volume analysis
* Retailer-level performance
* Market-level composition
* Order method comparison
* KPI calculations
* Ranking and segmentation of business entities

The resulting query outputs were then used as the data source for the visualization layer.

---

# Dashboard

The analytical results were connected to **Looker Studio / Google Data Studio** to create an interactive business dashboard.

The dashboard was designed to allow users to explore the results without needing to write SQL or directly access BigQuery.

### Dashboard objectives

The dashboard provides an accessible view of:

* Overall sales performance
* Market composition
* Retailer contribution
* Order method performance
* Key business KPIs
* Areas requiring further investigation

---

# Key Analytical Areas

## Market Composition

The market analysis was designed to distinguish between markets dominated by a small number of major retailers and markets with a more fragmented retailer structure.

This provides a basis for considering different commercial strategies depending on market structure.

### Potential strategy

**Concentrated markets**

Focus on increasing sales volume with existing major retailers.

**Competitive markets**

Focus on expanding the retailer base and increasing market activity.

---

## Order Method Performance

Different order methods were compared based on their contribution to overall business activity.

The analysis considered both:

* Order volume
* Sales contribution

This provides a starting point for identifying order methods that may warrant further investigation from a cost-benefit perspective.

---

# Business Value

The project demonstrates how raw operational data can be transformed into a decision-support solution.

Instead of relying on disconnected CSV files, the workflow creates:

**Structured data → centralized analytics → automated SQL analysis → interactive reporting → business insights**

This makes the analysis more accessible to non-technical stakeholders and provides a foundation for repeatable business reporting.

---

# What I Learned

This project strengthened my practical understanding of the complete analytics workflow, including:

* Working with raw business data
* Structuring data for analytical use
* Using BigQuery as a cloud data warehouse
* Writing SQL queries for business analysis
* Creating reusable analytical datasets
* Connecting cloud data to visualization tools
* Designing dashboards for non-technical stakeholders
* Translating analytical results into business questions and recommendations
* Communicating data through visual storytelling

---

# Project Architecture

```text
                  ┌─────────────────┐
                  │   Raw CSV Data  │
                  └────────┬────────┘
                           │
                           ▼
                  ┌─────────────────┐
                  │    BigQuery     │
                  │  Data Warehouse │
                  └────────┬────────┘
                           │
                           ▼
                  ┌─────────────────┐
                  │   SQL Analysis  │
                  │                 │
                  │ • Market        │
                  │ • Retailers     │
                  │ • Orders        │
                  │ • KPIs          │
                  └────────┬────────┘
                           │
                           ▼
                  ┌─────────────────┐
                  │  Looker Studio  │
                  │    Dashboard    │
                  └────────┬────────┘
                           │
                           ▼
                  ┌─────────────────┐
                  │ Business        │
                  │ Insights        │
                  └─────────────────┘
```

---

# Project Deliverables

* BigQuery data warehouse
* SQL analysis queries
* Analytical datasets
* Interactive Looker Studio dashboard
* Market composition analysis
* Order method performance analysis
* Business-oriented KPI reporting

---

# Portfolio Context

This project was completed as part of my practical Data Analytics training and represents an end-to-end business analytics case study.

It demonstrates my ability to combine **cloud data warehousing, SQL, data analysis and visualization** to turn raw data into information that can support business decisions.

---

## Tools

`Google BigQuery` `SQL` `Looker Studio` `Google Sheets` `Data Analytics` `Data Visualization` `Business Intelligence`

---

## Author

**Dr. rer. nat. Tovhowani Innocent Kwinda**

Data Analytics | Business Analytics | Process Optimization | Technical Chemistry

E-mail: [kwindati@gmail.com]

---

## Note on Data

The project dataset was provided as part of the case study. The repository focuses on the analytical workflow, SQL logic, visualizations and project documentation rather than redistribution of the original source data.
