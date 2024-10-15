# Data Quality Management and Staff Dashboard Visualisation

#### Date: 2024-09-19

This project presents a technical solution for a data analysis assessment for a job position at a Singapore public agency. The task focuses on **processing access data, addressing data quality issues**, and **creating interactive dashboards** to monitor and analyse staff attendance patterns and remote work targets.

## Table of Contents
- [Overview](#overview)  
- [Data Preparation](#data-preparation)  
- [Dashboard Insights](#dashboard-insights)  
- [Code Structure](#code-structure)  
- [Assumptions](#assumptions)  
- [License](#license)
<!--- [How to Use](#how-to-use)  -->
---

## Overview
The purpose of this project is to:
1. **Process and clean** the building access data provided by Company XYZ.
2. **Identify data quality issues** and implement fixes to ensure the data is ready for analysis.
3. **Create visual dashboards** that help monitor:
   - Percentage of staff working from home.
   - Distribution of staff attendance across time slots.
   - Issuance of temporary and visitor passes at different office sites.

## Data Preparation
- **Datasets**: This project uses 22 CSV files representing building access logs and a data dictionary.
- **Data Quality Checks**:  
  - Correcting column names and formats.
  - Handling missing or invalid values.
  - Removing duplicate entries (keeping only the earliest entry per day).
  - Ensuring numeric consistency for card numbers.

The processed dataset will allow future ingestion of new data without requiring significant rework.

## Dashboard Insights
The dashboard provides actionable insights in three key areas:
1. **Staff Working from Home**:
   - Tracks daily percentages of employees working remotely to meet a target of 80%.
2. **Staff Attendance Patterns**:
   - Monitors the number of days staff come into the office each week.
   - Analyzes arrival time slots to ensure an even distribution across:
     - **07:00 – 08:29**
     - **08:30 – 09:29**
     - **09:30 – 10:30**
3. **Visitor and Temporary Pass Usage**:
   - Visualizes the number of Temp and Visitor pass holders at each office site.

The combined dashboard is available on Tableau Public, https://public.tableau.com/views/ABC-Staff-Dashboard/Dashboard

## Code Structure
The following files are included in this repository:

```bash
Job-Assessments/
│
└── Data-Quality_Staff-Dashboard/
    ├── Data-Quality-Staff-Dashboard.md                     # Markdown file containing the code, plots and explanations
    ├── Data-Quality-Staff-Dashboard.Rmd                    # R Markdown file containing the code and explanations
    ├── Access_data/                                        # Directory containing CSV files for building access logs
    ├── Data-Quality-Staff-Dashboard_files/figure-gfm/      # Directory to store generated plots
    └── README.md                                           # This README file
```

## Assumptions
- Only the first tap-in entry per day is considered for attendance analysis.
- Invalid card numbers (e.g., `#REF!` or `#VALUE!`) are replaced with `Unknown`.
- Missing department names are labeled as `Dept Unknown`.
- All Temp and Visitor pass holders are treated equally across the sites.

## License
This project is intended for submission as part of a technical assessment. The content and code are not intended for public or commercial use without explicit permission.
