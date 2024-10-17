# Compute Average Monthly Wage by Firm Size

#### Date: 2024-09-18

## Introduction  
**Brief Overview:**
This project demonstrates how to compute the average monthly wage paid by companies of different sizes using R. The analysis uses simulated data based on two hypothetical tables provided in the job application assessment: one representing companies and the other representing employee wage data. The R Markdown (RMD) code is structured to simulate data loading, define firm sizes, and compute the average monthly wage for each firm size.

This project was undertaken as part of a job application assessment for a job position with a Singapore public agency. The code simulates data analysis using R to demonstrate the ability to manipulate and analyse datasets, despite no actual CSV files being provided.

**Objectives:**  
- Simulate the computation of average monthly wages based on firm size (small, medium, large).
- Simulate merging two datasets (companies and employees) for analysis.
- Provide a clean and reproducible workflow using R Markdown to showcase data analysis skills.

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
**Prerequisites:**
- R (version 4.0 or above)
- RStudio

**Evironment Setup:**
1. Install R from the CRAN website.
2. Install RStudio from RStudio website.
3. Ensure that you have the following R packges installed:
```r
install.packages("tidyverse")
```

**Dependencies:**
- `tidyverse`: A collection of R packages for data manipulation and visualization.

## Usage
**Instructions:**
1. Clone or download the repository from GitHub.
2. Navigate to the `Calc-Avg-Mthly-Wage` folder.
3. Open the `Calc-Avg-Mthly-Wage.Rmd` file in RStudio.

## Data
**Data Sources:**
- The data used in this project is simulated based on the tables provided in the job application assessment. No actual CSV files were given.

**Data Description:**
- Companies Dataset:
  - `Company_Name`: Unique identifier for each company.
  - `Date_of_Incorporation`: Date when the company was established.
  - `Revenue`: Company revenue (in dollars).
  - `Sector`: Industry sector.
- Employees Dataset:
  - `Employee_Name`: Unique identifier for each employee.
  - `Company_Name`: Name of the company the employee works for.
  - `Monthly_Wage`: Monthly salary of the employee (in dollars).

**Data Processing:**
- Simulated data was created based on the provided tables.
- Company sizes were defined based on revenue categories, which are assumptions made for the analysis.
- The datasets were merged by Company_Name to link employees to their respective companies.
- The average monthly wage for each company size category was computed.

## Methodology
**Techniques Used:**
- **Data Simulation:** The data was simulated based on the tables provided in the job assessment.
- **Data Cleaning and Merging:** Dataframes were merged based on the `Company_Name` column to associate employees with companies.
- **Group by Firm Size:** Firms were categorised into small, medium, and large based on their revenue, and the average wage for each group was calculated.

**Tools:**
- **R:** For data analysis and computation.
- **tidyverse:** For data manipulation and summarization.
- **RMarkdown:** For creating reproducible analysis and reporting.

## Results
**Findings:**
The average monthly wage for each firm size (small, medium, large) was calculated using the simulated dataset. These results provide insights into the wage distribution across firms of different sizes.

**Visualisations:**
A summary table of average wages by firm size is printed in the R Markdown document.

**Interpretation:**
- **Small Firms:** Firms with revenue under $1,500,000.
- **Medium Firms:** Firms with revenue between $1,500,000 and $2,000,000.
- **Large Firms:** Firms with revenue above $2,000,000.

## Project Structure
**Directory Tree:**
```markdown
Calc-Avg-Mthly-Wage/
│
├── Calc-Avg-Mthly-Wage.Rmd
└── README.md
```

**Key Files:**
- **Calc-Avg-Mthly-Wage.Rmd:** The R Markdown file containing the code for data analysis.
- **README.md:** This document, providing details on how to use and understand the project.

## License
This project is intended for submission as part of a technical assessment. The content and code are not intended for public distribution, reproduction, or commercial use without explicit permission from the Author.

## Contact Information
- **Author:** Ou Yang Yu
