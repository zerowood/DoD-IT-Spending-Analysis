# DoD IT Spending Analysis (FY2025)
**Author:** Zee Wood Alston | **Portfolio:** [zerowood](https://github.com/zerowood)
**Data Source:** USAspending.gov API (PSC Category D)

## Executive Overview
This project provides a reproducible data pipeline for auditing **$41.9 Billion** in Department of Defense IT spending. By extracting real-time contract obligations, the analysis identifies the distribution of funds across sub-agencies and categorizes investment into **Modernization (DME)** vs. **Maintenance (O&M)**.

## Technical Stack
* **Language:** Python 3.x (Conda Env: `private_ai`)
* **Libraries:** Pandas, Plotly Express, NumPy, Requests
* **Automation:** Integrated Git/PowerShell workflow for artifact persistence.

## Repository Structure
* `/notebooks`: Contains the core `.ipynb` with environment validation and fallback API logic.
* `/it_spending_analysis_outputs`: 
    * `dod_it_spending_report.html`: Interactive Treemap (Exponent-free formatting).
    * `dod_it_cleaned_data.csv`: Normalized dataset for secondary BI analysis.
    * `dod_it_audit_*.csv`: Timestamped audit trails (ignored by Git, available locally).

## Key Features
1. **Defensive API Ingestion:** Built-in fallback logic to handle government reporting latency and naming conventions (e.g., "Department of Defense" vs "(DOD)").
2. **The "Exponent Killer":** Custom lambda-formatting to ensure high-value billions ($5.67B) render correctly for executive review.
3. **Median-Split Heuristics:** Automated categorization of sub-agencies based on investment weight to distinguish legacy support from new development.

## How to Run
1. Clone the repo.
2. Ensure `Pandoc` is installed for high-spec report generation.
3. Run `notebooks/federal_agencies_spend_treemap.ipynb`.