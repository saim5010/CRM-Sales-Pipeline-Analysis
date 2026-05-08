# 📊 CRM Sales Pipeline Analysis

A comprehensive exploration of a B2B sales pipeline dataset covering **4,238 closed-won opportunities** across 30 sales agents, 3 regional offices, and 7 product lines throughout 2017.

---

## 📁 Repository Structure

```
CRM-Sales-Pipeline-Analysis/
│
├── crm_sales_pipeline.xlsx       # Raw dataset (pivot summaries + transaction records)
├── README.md                     # Project documentation
```

---

## 🗂️ Dataset Overview

The dataset spans the full 2017 fiscal year and contains three interconnected data layers:

| Layer | Description |
|---|---|
| **Transaction Records** | Row-level opportunity data with agent, product, account, dates, and close value |
| **Pivot Summaries** | Quarterly aggregations of Won/Lost counts by agent and deal stage |
| **Org Hierarchy** | Agent → Manager → Regional Office mapping for all 35 sales personnel |

### Column Definitions

| Column | Type | Description |
|---|---|---|
| `opportunity_id` | String | Unique 8-character alphanumeric identifier per deal |
| `sales_agent` | String | Name of the sales representative handling the opportunity |
| `manager` | String | Direct manager of the sales agent |
| `regional_office` | String | One of three regions: Central, East, or West |
| `product` | String | Product line sold (7 variants — see below) |
| `account` | String | Client/company name |
| `deal_stage` | String | Final outcome: `Won`, `Lost`, or `Engaging` (still open) |
| `engage_date` | Date | Date the opportunity was first initiated |
| `close_date` | Date | Date the deal was closed (null if still Engaging) |
| `close_value` | Integer | Revenue generated in USD (0 for Lost; null if Engaging) |

---

## 🏢 Organizational Structure

The sales force is divided across **3 regional offices**, each managed by **2 managers** overseeing ~5–6 agents:

| Region | Managers |
|---|---|
| Central | Dustin Brinkmann, Melvin Marxen |
| East | Cara Losch, Rocco Neubert |
| West | Celia Rouche, Summer Sewald |

---

## 🛒 Product Lines

| Product | Tier |
|---|---|
| GTX Basic | Entry |
| GTX Plus Basic | Entry-Mid |
| GTXPro | Mid |
| GTX Plus Pro | Mid-High |
| MG Special | Entry |
| MG Advanced | Mid-High |
| GTK 500 | Premium |

---

## 📈 Key Metrics at a Glance

| Metric | Value |
|---|---|
| Total Won Deals | 4,238 |
| Total Lost Deals | 2,473 |
| Overall Win Rate | ~63% |
| Active (Engaging) Deals | Present in dataset |
| Top Sales Agent | Darcel Schlecht (349 won deals) |
| Date Range | October 2016 (engage) → December 2017 (close) |
| Highest Single Deal | $25,897 — GTK 500, Elease Gluck |

### Quarterly Trend (Won Deals)

| Quarter | Won Deals |
|---|---|
| Q1 2017 | 531 |
| Q2 2017 | 1,254 |
| Q3 2017 | 1,257 |
| Q4 2017 | 1,196 |
| **Total** | **4,238** |

---

## 🔍 Potential Analysis Directions

- **Win Rate Analysis** — by agent, product, manager, and region
- **Revenue Attribution** — which product lines and agents drive the most close value
- **Sales Cycle Duration** — average days from `engage_date` to `close_date` by deal stage and product
- **Agent Performance Benchmarking** — ranking agents within their region and manager cohort
- **Lost Deal Patterns** — identifying which products, accounts, or agents have the highest loss rates
- **Pipeline Health** — proportion of Engaging deals and their projected conversion potential

---

## 🛠️ Tools & Technologies

This dataset is well-suited for analysis using:

- **Python** — Pandas, Matplotlib, Seaborn for EDA and statistical analysis
- **SQL** — Aggregations, window functions, self-joins for pipeline metrics
- **Power BI / Tableau** — Interactive dashboards with slicers by region, product, and agent
- **Excel** — Pivot tables, conditional formatting, basic dashboarding

---

## 👤 Author

**Saim Mulani**
Data Analyst & BI Developer | Pune, Maharashtra

[![LinkedIn](https://img.shields.io/badge/LinkedIn-saimmulani--data-blue?style=flat&logo=linkedin)](https://linkedin.com/in/saimmulani-data)
[![GitHub](https://img.shields.io/badge/GitHub-saim5010-black?style=flat&logo=github)](https://github.com/saim5010)

---

## 📄 License

This dataset is used for portfolio and educational purposes.# 📊 CRM Sales Pipeline Analysis

A comprehensive exploration of a B2B sales pipeline dataset covering **4,238 closed-won opportunities** across 30 sales agents, 3 regional offices, and 7 product lines throughout 2017.

---

## 📁 Repository Structure

```
CRM-Sales-Pipeline-Analysis/
│
├── crm_sales_pipeline.xlsx       # Raw dataset (pivot summaries + transaction records)
├── README.md                     # Project documentation
```

---

## 🗂️ Dataset Overview

The dataset spans the full 2017 fiscal year and contains three interconnected data layers:

| Layer | Description |
|---|---|
| **Transaction Records** | Row-level opportunity data with agent, product, account, dates, and close value |
| **Pivot Summaries** | Quarterly aggregations of Won/Lost counts by agent and deal stage |
| **Org Hierarchy** | Agent → Manager → Regional Office mapping for all 35 sales personnel |

### Column Definitions

| Column | Type | Description |
|---|---|---|
| `opportunity_id` | String | Unique 8-character alphanumeric identifier per deal |
| `sales_agent` | String | Name of the sales representative handling the opportunity |
| `manager` | String | Direct manager of the sales agent |
| `regional_office` | String | One of three regions: Central, East, or West |
| `product` | String | Product line sold (7 variants — see below) |
| `account` | String | Client/company name |
| `deal_stage` | String | Final outcome: `Won`, `Lost`, or `Engaging` (still open) |
| `engage_date` | Date | Date the opportunity was first initiated |
| `close_date` | Date | Date the deal was closed (null if still Engaging) |
| `close_value` | Integer | Revenue generated in USD (0 for Lost; null if Engaging) |

---

## 🏢 Organizational Structure

The sales force is divided across **3 regional offices**, each managed by **2 managers** overseeing ~5–6 agents:

| Region | Managers |
|---|---|
| Central | Dustin Brinkmann, Melvin Marxen |
| East | Cara Losch, Rocco Neubert |
| West | Celia Rouche, Summer Sewald |

---

## 🛒 Product Lines

| Product | Tier |
|---|---|
| GTX Basic | Entry |
| GTX Plus Basic | Entry-Mid |
| GTXPro | Mid |
| GTX Plus Pro | Mid-High |
| MG Special | Entry |
| MG Advanced | Mid-High |
| GTK 500 | Premium |

---

## 📈 Key Metrics at a Glance

| Metric | Value |
|---|---|
| Total Won Deals | 4,238 |
| Total Lost Deals | 2,473 |
| Overall Win Rate | ~63% |
| Active (Engaging) Deals | Present in dataset |
| Top Sales Agent | Darcel Schlecht (349 won deals) |
| Date Range | October 2016 (engage) → December 2017 (close) |
| Highest Single Deal | $25,897 — GTK 500, Elease Gluck |

### Quarterly Trend (Won Deals)

| Quarter | Won Deals |
|---|---|
| Q1 2017 | 531 |
| Q2 2017 | 1,254 |
| Q3 2017 | 1,257 |
| Q4 2017 | 1,196 |
| **Total** | **4,238** |

---

## 🔍 Potential Analysis Directions

- **Win Rate Analysis** — by agent, product, manager, and region
- **Revenue Attribution** — which product lines and agents drive the most close value
- **Sales Cycle Duration** — average days from `engage_date` to `close_date` by deal stage and product
- **Agent Performance Benchmarking** — ranking agents within their region and manager cohort
- **Lost Deal Patterns** — identifying which products, accounts, or agents have the highest loss rates
- **Pipeline Health** — proportion of Engaging deals and their projected conversion potential

---

## 🛠️ Tools & Technologies

This dataset is well-suited for analysis using:

- **Python** — Pandas, Matplotlib, Seaborn for EDA and statistical analysis
- **SQL** — Aggregations, window functions, self-joins for pipeline metrics
- **Power BI / Tableau** — Interactive dashboards with slicers by region, product, and agent
- **Excel** — Pivot tables, conditional formatting, basic dashboarding

---

## 👤 Author

**Saim Mulani**
Data Analyst & BI Developer | Pune, Maharashtra

[![LinkedIn](https://img.shields.io/badge/LinkedIn-saimmulani--data-blue?style=flat&logo=linkedin)](https://linkedin.com/in/saimmulani-data)
[![GitHub](https://img.shields.io/badge/GitHub-saim5010-black?style=flat&logo=github)](https://github.com/saim5010)

---
