# Data Quality and Staff Dashboard Visualisation

#### Date: 2024-09-19

## Introduction

### Brief Overview
This project focuses on organising and cleaning access data from Company ABC and developing an interactive dashboard to monitor staff attendance patterns. The dashboard provides insights into staff working from home, office arrival time slots, and visitor access trends, supporting informed decision-making.

This project was developed in response to a technical assessment for a job role with a Singapore public agency. The goal is to clean and manage data, identify quality issues, and create effective visualisations for tracking key metrics.

### Objectives
1. Clean and process raw data from access logs to ensure data quality.
2. Develop a scalable data ingestion solution for future datasets.
3. Create a dashboard that provides insights into:
   - Staff working-from-home trends.
   - Distribution of staff arrival times.
   - Visitor and temporary pass usage across office sites.

---

## Table of Contents
- [Introduction](#introduction)
- [Installation](#installation)
- [Usage](#usage)
- [Data](#data)
- [Methodology](#methodology)
- [Results](#results)
- [Project Structure](#project-structure)
- [License](#license)
- [Contact Information](#contact-information)

---

## Installation

### Prerequisites
- R (version 4.0 or higher)
- RStudio

<!--
**Environment Setup:**
1. Clone this repository:
    ```bash
    git clone https://github.com/Gyres/Job-Assessments.git
    cd Job-Assessments/Data-Quality_Staff-Dashboard
    ```
2. Open Data-Quality_Staff-Dashboard.Rmd in RStudio.
-->

**Dependencies:**
Install the required R packages:

```r
install.packages(c("tidyverse", "lubridate", "flexdashboard", "plotly"))
```

---

## Usage
**Instructions:**
1. Access [Data-Quality_Staff-Dashboard.md](Data-Quality_Staff-Dashboard.md) to view the pre-run analysis.

    or

2. Open Data-Quality_Staff-Dashboard.Rmd file from within RStudio.
3. Knit the file to generate an HTML report. Alternatively, run the code chunks sequentially to reproduce the analysis.
4. The dashboard will generate:
   - Daily percentage of staff working from home.
   - Histogram showing staff attendance patterns per week.
   - Time slot distribution of staff arrivals.
   - Bar chart of visitor and temporary pass usage across office sites.

The combined dashboard is available on Tableau Public, https://public.tableau.com/views/ABC-Staff-Dashboard/Dashboard

---

## Data
**Data Sources**
- **Access_data:** Provided by Company ABC, containing access logs of two office sites.

**Data Description**
- **When:** Timestamp of access.
- **Profile:** Type of pass (Staff, Temp, Visitor).
- **Dept:** Department name.
- **CardNum:** Unique identifier for staff.

**Data Processing**
1. Corrected column names and removed unnecessary spaces.
2. Replaced missing values and handled invalid data formats.
3. Filtered data to keep only the first entry per day for each individual.

---

## Methodology
**Techniques Used**
- Data cleaning and wrangling using tidyverse.
- Dashboard creation with flexdashboard and plotly.

**Tools**
- RStudio for development and testing.
- R for data manipulation and visualisation.

---

## Results
**Findings**
- 80% Work-from-Home Target: Achieved on most days based on access logs.
- Work-from-Office Patterns: Most Staff come into office at least once per week.
- Time Slot Distribution: Most staff arrive between 7:00 and 9:29 AM.
- Visitor Pass Insights: More visitor passes issued at Site A.

**Visualisations**
1. Daily Work-from-Home Percentage
2. Number of days Staff Work-from-Office per week Distribution
3. Arrival Time Slot Distribution
4. Number of Temporary and Visitor Pass by Site

---

## Project Structure
```bash
Data-Quality_Staff-Dashboard/
│
├── README.md                                        # Project overview and instructions
├── Data-Quality_Staff-Dashboard.md                  # Main analysis report
├── Data-Quality_Staff-Dashboard.Rmd                 # Main analysis script
├── Access_data/                                     # Directory containing CSV files for building access logs
└── Data-Quality-Staff-Dashboard_files/figure-gfm/   # Directory to store generated plots
```

---

## License

This project is intended for submission as part of a technical assessment. The content and code are not intended for public distribution, reproduction, or commercial use without explicit permission from the Author.

---

## Contact Information

**Author:** Ou Yang Yu
