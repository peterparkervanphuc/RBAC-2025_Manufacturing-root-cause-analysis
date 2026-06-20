# Toothbrush Manufacturing Throughput Analysis (RBAC 2025)

This portfolio project investigates manufacturing inefficiencies in a toothbrush factory, with a focus on machine downtime and product defects. The work was prepared for the RBAC 2025 analytics challenge and packaged here for recruiters and hiring teams to review my end-to-end analytics workflow.

## Business Context

The factory is losing throughput due to:

- Frequent machine downtime events.
- Defective output concentrated in specific lines/products.

Goal: identify root causes, quantify operational impact, and propose practical improvement actions.

## Project Scope

I addressed four core questions:

1. Performance overview (OEE, Defect Rate, Throughput Yield).
2. Root cause analysis for downtime and defect patterns.
3. Business impact quantification (lost units, waste implications).
4. Actionable recommendations for throughput and quality improvement.

## What I Did

1. Data integration and cleaning from three source files (`production_logs`, `maintenance_order`, `cross_reference`).
2. Feature engineering and aggregation at shift/line/date level.
3. KPI modeling for `Availability`, `Performance`, `Quality`, `OEE`, `Defect Rate`, and `Throughput Yield`.
4. Deep EDA to locate repeated and emerging issues by line, shift, and product grouping.
5. Root-cause storytelling with slide-based investigation artifacts.
6. Dashboarding in Power BI for stakeholder communication.

## Key Investigation Highlights

From the submitted Q2 investigation documents and final presentation:

- Downtime concentration was investigated around MKBC lines, with repeated references to a "Handle Jam" issue.
- Defect concentration was investigated on MAFT lines, with emphasis on low-quality output related to the "Renew 360" product stream.
- Maintenance scheduling quality was treated as a contributing factor in recurring losses.

## Achievements
- Top 30 competition

## Repository Structure

```text
.
|-- data/
|   |-- raw/
|   |   |-- production_logs.csv
|   |   |-- maintenance_order.csv
|   |   `-- cross_reference.csv
|   `-- processed/
|       `-- master_data.csv
|-- notebooks/
|   |-- 01_data_integration_and_cleaning.ipynb
|   |-- 02_exploratory_data_analysis.ipynb
|   |-- 03_kpi_calculation_q1.ipynb
|   |-- 04_root_cause_analysis_q2.ipynb
|   `-- 99_legacy_analysis_unrelated.ipynb
|-- dashboards/
|   `-- powerbi/
|       `-- Manufacturing_Performance_Dashboard.pbix
|-- reports/
|   `-- slides/
|       |-- PROBAI_Round_2_RBAC_2025_Final.pdf
|       |-- Q2_Root_Cause_Detailed_Investigation.pdf
|       `-- Q2_Root_Cause_Quick_Version.pdf
`-- README.md
```

## How to Reproduce (Notebook Flow)

1. Open `notebooks/01_data_integration_and_cleaning.ipynb` to understand preprocessing and the creation logic for master data.
2. Continue with `notebooks/02_exploratory_data_analysis.ipynb` for pattern discovery and root-cause exploration.
3. Run `notebooks/03_kpi_calculation_q1.ipynb` for KPI computation and summary metrics.
4. Run `notebooks/04_root_cause_analysis_q2.ipynb` for the detailed Q2 root-cause investigation storyline.
5. Open the Power BI file in `dashboards/powerbi/` for presentation-ready visualization.

## Skills Demonstrated

- Manufacturing analytics and KPI design.
- Data cleaning and robust merge strategy.
- Root cause analysis for operations.
- Business-impact framing.
- Executive storytelling with slides and dashboarding.

## Notes for Recruiters

This project reflects how I approach real operational data:

- Translate messy event logs into business KPIs.
- Connect analysis to root causes and practical actions.
- Deliver outputs in both technical notebooks and decision-friendly presentation formats.
