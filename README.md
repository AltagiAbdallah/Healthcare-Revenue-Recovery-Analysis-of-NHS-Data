# Healthcare Revenue Recovery: Analysis of NHS Data

![Python](https://img.shields.io/badge/Python-3.9%2B-blue)
![Pandas](https://img.shields.io/badge/Library-Pandas-green)
![Status](https://img.shields.io/badge/Analysis-Complete-success)

## Project Overview
This project focuses on **Healthcare Revenue Recovery** by analyzing NHS Hospital Episode Statistics (HES). It targets the systemic issue of "Did Not Attend" (DNA) appointments—outpatient slots that are booked but go unused.

By correlating operational data with financial modeling, this analysis quantifies the "Ghost Capacity" in the system and proposes strategies to recover lost revenue.

## The Business Problem
* **Operational Drag:** Missed appointments create gaps in provider schedules that cannot be refilled last minute.
* **Financial Leakage:** Each empty slot represents sunk costs in staffing and overhead (Est. £160/appointment).
* **The Goal:** To transform raw attendance logs into a strategic asset for revenue protection.

## Visual Insights
*(Key charts generated from the analysis)*

### 1. The Cost of Waste (Financial Dashboard)
**Insight:** The horizontal analysis reveals specific months where revenue leakage exceeded operational tolerance levels.
![Financial Loss Chart](https://github.com/AltagiAbdallah/Healthcare-Revenue-Recovery-Analysis-of-NHS-Data/blob/06d45742072acc295a69dbc4be3e01957b25d955/Charts/financial_loss_chart.png)

### 2. Operational Efficiency Trend
**Insight:** The DNA rate (blue line) shows the long-term reliability of patient attendance.
![Efficiency Trend Chart](https://github.com/AltagiAbdallah/Healthcare-Revenue-Recovery-Analysis-of-NHS-Data/blob/06d45742072acc295a69dbc4be3e01957b25d955/Charts/efficiency_trend.png)

## Technical Methodology
1.  **Data Sourcing:** Automated ingestion of NHS Consultation logs (Planned vs. Emergency).
2.  **Financial Modeling:**
    * **Metric:** `Revenue_Leakage` = `DNA_Volume` * `£160` (Avg. Tariff).
    * **Trend Analysis:** Identified seasonal spikes in non-attendance.
3.  **Visualization:** Developed a "Financial Waste Dashboard" to communicate the magnitude of loss to non-technical stakeholders.

## Key Findings
* **Total Recoverable Revenue:** Identified **>£15 Billion** (Aggregate) in potential revenue lost to DNAs across the reporting period.
* **Inefficiency Trend:** The DNA rate shows a clear correlation with specific operational periods, suggesting targeted intervention opportunities.

## How to Run
1.  **Clone the Repository:**
    ```bash
    git clone [https://github.com/yourusername/healthcare-revenue-recovery.git](https://github.com/yourusername/healthcare-revenue-recovery.git)
    ```
2.  **Install Requirements:**
    ```bash
    pip install pandas seaborn matplotlib opendatasets
    ```
3.  **Execute Analysis:**
    Open the Jupyter Notebook and run all cells to reproduce the financial audit.

