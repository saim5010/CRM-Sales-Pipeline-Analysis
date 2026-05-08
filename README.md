📊 CRM Sales Pipeline Analysis
A comprehensive exploration of a B2B sales pipeline dataset covering 4,238 closed-won opportunities across 30 sales agents, 3 regional offices, and 7 product lines throughout 2017.

📁 Repository Structure
CRM-Sales-Pipeline-Analysis/
│
├── crm_sales_pipeline.xlsx       # Raw dataset (pivot summaries + transaction records)
├── README.md                     # Project documentation

🗂️ Dataset Overview
The dataset spans the full 2017 fiscal year and contains three interconnected data layers:
LayerDescriptionTransaction RecordsRow-level opportunity data with agent, product, account, dates, and close valuePivot SummariesQuarterly aggregations of Won/Lost counts by agent and deal stageOrg HierarchyAgent → Manager → Regional Office mapping for all 35 sales personnel
Column Definitions
ColumnTypeDescriptionopportunity_idStringUnique 8-character alphanumeric identifier per dealsales_agentStringName of the sales representative handling the opportunitymanagerStringDirect manager of the sales agentregional_officeStringOne of three regions: Central, East, or WestproductStringProduct line sold (7 variants — see below)accountStringClient/company namedeal_stageStringFinal outcome: Won, Lost, or Engaging (still open)engage_dateDateDate the opportunity was first initiatedclose_dateDateDate the deal was closed (null if still Engaging)close_valueIntegerRevenue generated in USD (0 for Lost; null if Engaging)

🏢 Organizational Structure
The sales force is divided across 3 regional offices, each managed by 2 managers overseeing ~5–6 agents:
RegionManagersCentralDustin Brinkmann, Melvin MarxenEastCara Losch, Rocco NeubertWestCelia Rouche, Summer Sewald

🛒 Product Lines
ProductTierGTX BasicEntryGTX Plus BasicEntry-MidGTXProMidGTX Plus ProMid-HighMG SpecialEntryMG AdvancedMid-HighGTK 500Premium

📈 Key Metrics at a Glance
MetricValueTotal Won Deals4,238Total Lost Deals2,473Overall Win Rate~63%Active (Engaging) DealsPresent in datasetTop Sales AgentDarcel Schlecht (349 won deals)Date RangeOctober 2016 (engage) → December 2017 (close)Highest Single Deal$25,897 — GTK 500, Elease Gluck
Quarterly Trend (Won Deals)
QuarterWon DealsQ1 2017531Q2 20171,254Q3 20171,257Q4 20171,196Total4,238

🔍 Potential Analysis Directions

Win Rate Analysis — by agent, product, manager, and region
Revenue Attribution — which product lines and agents drive the most close value
Sales Cycle Duration — average days from engage_date to close_date by deal stage and product
Agent Performance Benchmarking — ranking agents within their region and manager cohort
Lost Deal Patterns — identifying which products, accounts, or agents have the highest loss rates
Pipeline Health — proportion of Engaging deals and their projected conversion potential


🛠️ Tools & Technologies
This dataset is well-suited for analysis using:

Python — Pandas, Matplotlib, Seaborn for EDA and statistical analysis
SQL — Aggregations, window functions, self-joins for pipeline metrics
Power BI / Tableau — Interactive dashboards with slicers by region, product, and agent
Excel — Pivot tables, conditional formatting, basic dashboarding


👤 Author
Saim Mulani
Data Analyst & BI Developer | Pune, Maharashtra

📄 License
This dataset is used for portfolio and educational purposes.
