# Hospital Emergency Room Dashboard
An Excel-based dashboard that visualizes key ER metrics such as total patients, average wait time, admission status, referral departments, age-group distribution, attendance timeliness, and gender-wise analysis for monthly reporting.[13]

## Overview
The dashboard provides an at-a-glance monthly view of emergency room performance, helping stakeholders monitor throughput, patient satisfaction, and referral patterns to guide operational decisions and resource allocation. Visuals include KPI tiles, bar and donut charts, slicers for month selection, and dynamic summaries designed for quick insights.[13]

## Features
- KPI tiles for No. of Patients, Average Wait Time, and Patient Satisfaction Score across selected months.[13]
- Interactive slicers to switch months and filter visuals consistently across the page.[13]
- Admission status summary (admitted vs. not admitted) and department referral breakdowns for operational context.[13]
- Age group disatribution (e.g., 0–9, 10–19, …) and attendance status (on-time vs. delay) for patient flow understanding.[13]
- Gender-wise analysis for equity and planning insights.[13]

## Getting started

### Prerequisites
- Microsoft Excel (Microsoft 365 or Excel 2019+ recommended for optimal slicer performance and compatibility).[13]
- Enable macros if the file includes VBA-driven refresh or navigation buttons (optional).[13]

### Installation
1) Download or clone this repository to a local folder:  
- Code > Download ZIP, or  
- git clone https://github.com/<user>/<repo>.git.[13]
2) Open Hospital_ER_Dashboard.xlsx in Excel; if prompted, enable editing and enable content/macros as required.[13]

### Run locally
- Open the Dashboard sheet; use the month slicer on the left to switch reporting periods (e.g., Jan–Dec).[13]
- If a data table is linked (e.g., Data! table or Power Query connection), press Refresh All to pull updated records before reviewing the dashboard.[13]

### Optional refresh flow
- If Power Query is used: Data > Refresh All; verify connection paths if the source files are moved; store raw files under /data to keep paths consistent.[13]
- If using a CSV import: replace /data/er_latest.csv with new data of the same schema and Refresh All.[13]

## Usage
- Filter by month to view the KPIs and charts for the chosen reporting period, then review department referrals to identify bottlenecks or unusual spikes.[13]
- Check admission status and attendance timeliness to spot operational delays; combine with age-group and gender charts for cohort-specific actions.[13]

## Data structure
- Minimum fields: visit_date/month, patient_id, wait_time_minutes, satisfaction_score, admitted_flag, referral_department, age, gender, attendance_status.[13]
- Keep column names stable to avoid breaking PivotTables, Slicers, or Power Query steps; if schema changes, update pivot sources and queries accordingly.[13]

## Project structure
- /Hospital_ER_Dashboard.xlsx — the primary Excel file with the dashboard and PivotTables.[13]
- /data/ — sample and latest datasets; keep filenames consistent for refresh automation.[13]
- /assets/ — screenshots or GIFs embedded in the README for quick preview.[13]

## Roadmap
- Short term:  
  - Add a Data Quality sheet with counts of missing values and outliers by month.[13]
  - Introduce a trend view across months for KPIs with conditional formatting.[13]
- Medium term:  
  - Add a Department Drilldown page with referral, wait, and admission metrics by specialty.[13]
  - Parameterize the date range to support rolling 30/90-day analyses.[13]
- Long term:  
  - Integrate Power Query to automate data ingestion from CSV or database sources.[13]
  - Add a macro button to export a monthly PDF report for stakeholders.[13]

## Contributing
- Issues: Open an issue describing the change, expected behavior, and screenshots if UI is affected.[13]
- Branching: Create a feature branch from main, commit with clear messages (feat:, fix:, docs:), and open a pull request referencing the issue number.[13]
- Excel conventions:  
  - Keep a single “Data” table as the source; do not hardcode values into PivotTables.[13]
  - Name ranges and PivotTables descriptively; avoid breaking field names used by slicers.[13]

## Acknowledgments
Thanks to hospital operations teams and data staff whose workflow insights guided the KPIs and visual structure used here.[13]

