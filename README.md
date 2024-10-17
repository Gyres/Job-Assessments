# Job Assessments

## Introduction
This repository contains projects completed as part of technical assessments for job applications. Each project showcases different data analysis skills using R and R Markdown, including data manipulation, statistical analysis, and data visualisation.

**Projects Included:**
1. Compute Average Monthly Wage by Firm Size
2. Data Quality and Staff Dashboard Visualisation
3. US States Grouping and Assault Rate Prediction

## Table of Contents
1. [Introduction](#introduction)
2. [Projects](#projects)
    - [Compute Average Monthly Wage by Firm Size](#compute-average-monthly-wage-by-firm-size)
    - [Data Quality and Staff Dashboard Visualisation](#data-quality-and-staff-dashboard-visualisation)
    - [US States Grouping and Assault Rate Prediction](#us-states-grouping-and-assault-rate-prediction)
4. [Installation](#installation)
5. [Usage](#usage)
6. [Project Structure](#project-structure)
7. [License](#license)
8. [Contact Information](#contact-information)

---

## Projects
### Compute Average Monthly Wage by Firm Size
**Folder:** `Calc-Avg-Mthly-Wage`

**Overview:**

This project demonstrates how to compute the average monthly wage paid by companies of different sizes using R. The analysis uses simulated data based on hypothetical company and employee wage tables. The code simulates data loading, defines firm sizes, merges datasets, and computes the average monthly wage for each firm size category.

**Objectives:**
- Simulate the computation of average monthly wages based on firm size (small, medium, large).
- Simulate merging two datasets (companies and employees) for analysis.
- Provide a clean and reproducible workflow using R Markdown.

**Instructions:**
- Navigate to the [Calc-Avg-Mthly-Wage](Calc-Avg-Mthly-Wage) folder.
- Follow the instructions in the project's README.

### Data Quality and Staff Dashboard Visualisation
**Folder:** `Data-Quality_Staff-Dashboard`

**Overview:**

This project focuses on organizing and cleaning access data from Company ABC and developing an interactive dashboard to monitor staff attendance patterns. The dashboard provides insights into staff working from home, office arrival time slots, and visitor access trends, supporting informed decision-making.

**Objectives:**
- Clean and process raw data from access logs to ensure data quality.
- Develop a scalable data ingestion solution for future datasets.
- Create a dashboard that provides insights into staff attendance and visitor trends.

**Instructions:**
- Navigate to the [Data-Quality_Staff-Dashboard](Data-Quality_Staff-Dashboard) folder.
- Follow the instructions in the project's README.

### US States Grouping and Assault Rate Prediction
**Folder:** `States-Grouping_Assault-Prediction`

**Overview:**

This project analyses socio-economic and crime data to group US states based on their characteristics and identify factors that significantly predict assault rates. The analysis includes clustering and regression techniques to understand socio-economic patterns and crime trends across the US.

**Objectives:**
- Group US states based on socio-economic and crime characteristics using clustering analysis.
- Identify significant predictors of assault rates through regression models.
- Provide data-driven insights into socio-economic disparities and crime rates.

**Instructions:**
- Navigate to the [States-Grouping_Assault-Prediction](States-Grouping_Assault-Prediction) folder.
- Follow the instructions in the project's README.

---

## Installation
**Prerequisites:**
- R (version 4.0 or above)
- RStudio

**General Dependencies:**

Each project utilizes various R packages for data analysis and visualization.

Install packages using:
```r
install.packages(c("tidyverse", "lubridate", "flexdashboard", "plotly", "cluster", "factoextra", "broom", "car", "ggcorrplot", "usmap"))
```

**Note:** Please refer to each project's README for specific dependencies and installation instructions.

## Usage
**Instructions:**
1. **Clone the Repository:**
    ```bash
    git clone https://github.com/Gyres/Job-Assessments.git
    cd Job-Assessments
    ```
2. **Select a Project:**
    - Navigate to the desired project folder.
    - Follow the instructions in that project's README to run the analysis.
4. **Running the Analysis:**
    - Open the `.Rmd` file in RStudio.
    - Install any missing packages if prompted.
    - Run the code chunks sequentially or knit the document to generate the report.

## Project Structure

```bash
Job-Assessments/
│
├── Calc-Avg-Mthly-Wage/
│   ├── Calc-Avg-Mthly-Wage.Rmd
│   └── README.md
│
├── Data-Quality_Staff-Dashboard/
│   ├── Data-Quality_Staff-Dashboard.Rmd
│   ├── Data-Quality_Staff-Dashboard.md
│   └── README.md
│
├── States-Grouping_Assault-Prediction/
│   ├── States-Grouping_Assault-Prediction.Rmd
│   ├── States-Grouping_Assault-Prediction.md
│   └── README.md
│
└── README.md  # This file
```

## License
This repository and its projects are intended for submission as part of technical assessments. The content and code are not intended for public distribution, reproduction, or commercial use without explicit permission from the author.

## Contact Information
**Author:** Ou Yang Yu

If you have any questions or need further information, please feel free to contact me.
