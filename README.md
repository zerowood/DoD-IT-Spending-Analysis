# Department of Defense IT Spending Analysis (FY2024-2025)

## Project Overview
This repository contains a programmatic analysis of Information Technology (IT) contract obligations across Department of Defense (DoD) sub-agencies. Using the USAspending.gov API, the pipeline extracts financial data and categorizes investments into Development, Modernization, and Enhancement (DME) versus Operations and Maintenance (O&M) portfolios.

## Key Technical Insights
* Data Scale: Analyzed over $41.9 Billion in federal IT contract obligations.
* Methodology: Implemented statistical median-split logic to identify agency-level investment intensity.
* Visualization: Developed hierarchical budget exploration tools using D3.js-based Treemaps.

## Technical Stack
* Language: Python (Pandas, Plotly, Requests)
* Pipeline: End-to-end automation from API ingestion to interactive HTML reporting.
* Governance: Automated data audit trails and standardized version control protocols.

## Directory Structure
* federal_agencies_spend_treemap.ipynb: Primary analysis and data processing logic.
* it_spending_analysis_outputs/: Processed data exports and visualization assets.
* .gitignore: Configured to exclude local audit logs and temporary data files.
