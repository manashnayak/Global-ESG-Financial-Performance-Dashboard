# Global-ESG-Financial-Performance-Dashboard

1. Global ESG & Financial Performance Dashboard

An interactive Power BI dashboard analyzing 11 years (2015–2025) of financial and ESG (Environmental, Social, Governance) performance data across 1,000 global companies spanning 9 industries and 7 regions.

2. 📊 Overview

This project turns a raw financial + ESG dataset into a fully interactive, multi-page business intelligence dashboard. It's built to answer real analytical questions: Which industries lead on profitability? Which lead on ESG? How does sustainability intensity vary once you normalize for company size? Which companies are the true top performers across both financial and ESG dimensions?
The dashboard is structured around a proper star-schema data model and 25+ custom DAX measures, covering time intelligence, ranking/Pareto analysis, What-If scenario modeling, and dynamic drill-through.

3. 🛠️ Tech Stack
Power BI Desktop — report design, data modeling, visualization
DAX (Data Analysis Expressions) — 25+ custom measures and calculated columns
Power Query — data import and transformation
Star Schema Data Modeling — fact/dimension table design

4. 🗂️ Data Sources
File	Description
FactPerformance.csv	Core fact table — 11,000 rows of yearly company-level performance: Revenue, Profit Margin, Market Cap, Growth Rate, ESG scores (Overall/Environmental/Social/Governance), and sustainability metrics (Carbon Emissions, Water Usage, Energy Consumption)
DimCompany.csv	Company dimension — 1,000 companies with Industry and Region attributes
DimDate.csv	Date dimension — Year, Quarter, and Year Label lookup (2015–2025)
DAX_Measures.txt	Full reference list of all DAX measures used in the model

5. 📄 Report Pages
Executive Summary — high-level KPIs, revenue trend, industry breakdown, regional performance map
Financial Performance — YoY growth trend, 5-year CAGR, profit margin vs. growth scatter analysis, top revenue companies
ESG Deep Dive — Environmental/Social/Governance score breakdowns by industry, ESG trend over time, ESG rankings
Sustainability / Intensity — carbon, water, and energy intensity normalized per $M revenue, enabling fair cross-company comparison
Rankings & Top Performers — combined ESG + profitability ranking, Pareto (80/20) revenue concentration analysis
Company Detail (Drill-Through) — single-company deep dive with dynamic, filter-driven page title

6. ✨ Features & Highlights
Star-schema data model with clean fact/dimension separation
25+ custom DAX measures, organized into structured display folders (Core Financial, Time Intelligence, ESG Scoring, Sustainability Intensity, Ranking/Pareto, Dynamic Titles)
Time intelligence: YoY growth, running totals, 5-year CAGR — with explicit handling of the 2015 baseline year to avoid misleading growth figures
Sustainability intensity metrics: carbon/water/energy per $M revenue, so companies of different sizes can be compared fairly
Top Performer flag: identifies companies ranking in the top 100 on both ESG score and profit margin simultaneously
Drill-through page with a dynamic title bound to SELECTEDVALUE(), updating automatically per company
Conditional formatting (color scales, KPI trend indicators) for at-a-glance interpretation
Interactive slicers and cross-filtering across Year, Industry, and Region on every page

7. Goal

To provide a unified, interactive view of corporate financial and ESG performance — enabling stakeholders to evaluate companies not just on profitability and growth, but on sustainability and governance, using a single, data-driven dashboard.

Specifically, the dashboard is designed to answer:

Which industries and regions lead on revenue, profitability, and growth?
How does ESG performance vary across industries, and is it improving over time?
How sustainable is a company relative to its size — using intensity metrics (carbon/water/energy per $M revenue) rather than raw totals, which would just reflect scale?
Which companies are true "top performers" — strong on both financial results and ESG, not just one or the other?

8. Screenshots
  Executive Summary Page 1
https://github.com/manashnayak/Global-ESG-Financial-Performance-Dashboard/blob/main/Executive%20Summary%20PAGE%201.png
