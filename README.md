# DoD IT Spending Analysis (FY2024-2025)

## 📊 Overview
This project provides a programmatic analysis of Information Technology (IT) spending across Department of Defense (DoD) sub-agencies. Using the USAspending.gov API, the pipeline extracts contract obligations and categorizes them into Development/Modernization (DME) and Operations/Maintenance (O&M) portfolios.

### Key Insights
* **Scale:** Analyzed over **$41.9 Billion** in IT contract obligations.
* **Categorization:** Implemented a statistical median-split to identify investment intensity.
* **Visualization:** Created an interactive D3-based Treemap for hierarchical budget exploration.

## 🛠️ Technical Implementation
* **Language:** Python (Pandas, Plotly, Requests)
* **Automation:** End-to-end pipeline from API ingestion to data visualization.
* **Governance:** Automated data audit trails with timestamped CSV exports.

## 📂 Structure
* `federal_agencies_spend_treemap.ipynb`: Core analysis and data processing.
* `it_spending_analysis_outputs/`: Processed data and interactive HTML report.
* `.gitignore`: Automated governance to exclude audit logs from version control.
