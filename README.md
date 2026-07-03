#  Smart Supply Chains — Unlocking Performance Insights with Power BI

Interactive BI dashboard built on the **DataCo Smart Supply Chain** dataset, developed as part of the *Erasmus — BI & Data Analytics* course (2LIG), supervised by **Dr. Hamdi Hassen** and **Dr. Ahlem Ayari** — ISGS Sousse, Academic Year 2025–2026.

##  Context

In today's data-driven economy, companies generate vast amounts of transactional data across their supply chain operations. Without the right tools to analyze this data, critical performance issues remain hidden and decisions are made on intuition rather than facts.

This project applies BI concepts to the analysis of a real-world e-commerce supply chain dataset, turning raw data into actionable insights.

##  Dataset

- **Source:** DataCo Smart Supply Chain — Kaggle (CC0 Public Domain)
- **Size:** 180,519 orders, 53 columns
- **Period:** January 2015 – January 2018
- **Scope:** Global e-commerce — 164 countries, multiple regions and product categories

##  Key Performance Indicators

| KPI | Target | Actual |
| On-Time Delivery Rate (OTDR) | ≥ 95% | **45.2%** |
| Average Lead Time | ≤ 4 days | 3.5 days |
| Order Fulfillment Rate | ≥ 90% | **33%** |
| Late Delivery Risk Rate | ≤ 10% | **54.82%** |
| Average Profit per Order | — | $21.11 |
| Total Orders / Late Orders | — | 66,000 / 36,000 |

##  Dashboard Pages (5)

### 1. Overview
A snapshot of all key supply chain KPIs through card visuals, a donut chart of delivery status breakdown, and a bar chart of orders by shipping mode. Three interactive slicers (Date, Region, Shipping Mode) allow dynamic filtering across all visuals.

### 2. Delivery Performance
Monthly OTDR trend with a reference line at the 95% target, making the performance gap immediately visible. A 3-month forecast using Power BI's built-in ETS algorithm projects that OTDR will remain flat without intervention. A clustered column chart compares Total Orders vs Late Orders by month.

### 3. Order Fulfillment & Risk
Analysis of order status distribution and late delivery risk by region — with a fulfillment rate of only 33% and 54.82% of orders flagged as high delivery risk.

### 4. Shipping Mode Analysis
A detailed comparison of the four shipping modes reveals a striking paradox: **First Class**, despite having the shortest lead time (2 days), achieves the worst OTDR of only 5%, while **Standard Class** leads with 62% OTDR and $8M in sales.

### 5. Cost & Profit Analysis + What-If
Revenue and profitability analysis by region and product category, including an interactive **What-If simulator**. Using a slider parameter (0–30% cost reduction), users can simulate annual savings from reducing shipping costs — a 15% reduction yields approximately $1.9M in annual savings.

##  Key Findings

- OTDR of 45.2% — 36,000 out of 66,000 orders arrive late, far below the 95% target
- First Class shipping achieves only 5% OTDR despite a 2-day lead time — delivery promises are unachievable
- Standard Class is the most reliable (62% OTDR) and most profitable ($8M in sales) shipping mode
- Only 33% of orders reach COMPLETE status — a major processing backlog needs urgent attention
- 1,500 SUSPECTED_FRAUD orders represent unmonitored revenue risk
- Western Europe leads in sales ($2.3M); Q4 shows a clear seasonal profit peak

##  Recommendations

- Renegotiate or suspend First Class SLAs — the service is consistently failing
- Reduce PROCESSING backlog — streamline order management workflows
- Promote Same Day shipping for high-value orders — best lead time at 0.5 days
- Pre-position inventory ahead of Q4 seasonal demand peak
- Implement automated fraud detection to recover 1,500 at-risk orders
- Target 15% shipping cost reduction to unlock $1.9M annual savings

**Expected Impact:** OTDR 45.2% → 60–65% | Fulfillment Rate 33% → 55%+ | Late Orders -33% | Avg Profit/Order $21 → $25+

##  Tools Used

Power BI Desktop • Power Query (M) • DAX • `Dim_Calendar` table • ETS Forecasting • What-If Parameter

##  Repo Contents

```
├── SmartSupplyChain_PowerBI_MalekOueslatiG5B.pbix   # Power BI file
├── Rapport_BI_Oueslati_Malek.docx                # Full technical report
└── screenshots/                                       # Screenshots of the 5 pages
```

##  Author

**Oueslati Malek** 
