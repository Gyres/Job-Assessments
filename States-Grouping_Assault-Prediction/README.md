# US States Grouping and Assault Rate Prediction

#### Date: 2024-09-20

## Introduction  
**Brief Overview:**  
This project analyses socio-economic and crime data from various datasets to group US states based on their characteristics and identify factors that significantly predict assault rates. It was undertaken as part of a technical assessment for a job application at Singapore public agency.  

The goal was to demonstrate analytical and statistical skills, including clustering and regression analysis, in the context of real-world data challenges. Insights from this project can aid in understanding socio-economic patterns and crime trends across the US.  

**Objectives:**  
- **Group US states** based on socio-economic and crime characteristics using clustering analysis.  
- **Identify significant predictors** of assault rates through regression models.  
- Provide **data-driven insights** to better understand socio-economic disparities and crime rates.

---

## Table of Contents  
1. [Introduction](#introduction)  
2. [Installation](#installation)  
3. [Usage](#usage)  
4. [Data](#data)  
5. [Methodology](#methodology)  
6. [Results](#results)  
7. [Project Structure](#project-structure)  
8. [License](#license)   
9. [Contact Information](#contact-information)  

---

## Installation  
**Prerequisites:**  
- R version 4.0+  
- RStudio 

<!--
**Environment Setup:**
1. Clone this repository:
    ```bash
    git clone https://github.com/Gyres/Job-Assessments.git
    cd Job-Assessments/States-Grouping_Assault-Prediction
    ```
2. Open the RStudio project or .Rmd file in the States-Grouping_Assault-Prediction folder.
-->

**Dependencies:**
Install the required R libraries by running the following in R:

```r
install.packages(c("tidyverse", "cluster", "factoextra", "broom", "car", "ggcorrplot", "usmap"))
```

---

## Usage
**Instructions:**
1. Access [States_Grouping_Assault_Prediction.md](States-Grouping_Assault-Prediction.md) to view the pre-run analysis.

    or

2. Download the folder, States_Grouping_Assault_Prediction.
3. Open States_Grouping_Assault_Prediction.Rmd in RStudio.
4. Knit the file to generate an HTML report. Alternatively, run the code chunks sequentially to reproduce the analysis.

---

## Data
**Data Sources:**
- **USArrest.csv:** Contains crime data, including assault rates, for US states.
- **USstatex77.csv:** Includes socio-economic indicators for US states.

**Data Description:**
- **USArrest.csv:** Columns include `Murder`, `Assault`, `UrbanPop`, and `Rape`.
- **USstatex77.csv:** Contains indicators like `Population`, `Income`, `Illiteracy`, and `Life Expectancy`.

**Data Processing:**
- Merged multiple datasets on the `State` column.
- Normalised numeric variables for clustering.
- Handled missing data and multicollinearity issues for regression analysis.

---

## Methodology
**Techniques Used:**
- **Clustering Analysis:** Grouped states using K-means clustering with 4 clusters.
- **Regression Analysis:** Identified significant predictors of assault rates using multiple linear regression.

**Tools:**
- **Programming Languages:** R
- **Libraries:** tidyverse, cluster, factoextra, ggcorrplot, car, usmap

---

## Results
**Findings:**
- **Cluster Profiles:** States were grouped into clusters based on crime rates, income, urbanization, and education.
- **Regression Insights:** Higher urban population, higher rape rates, and lower life expectancy were associated with higher assault rates.

**Visualisations:**
- **Cluster Visualization:** Principal Component Analysis (PCA) plot showing clusters.
- **Correlation Matrix:** Displays relationships among variables.

**Interpretation:**
- Policies targeting urban population management and crime reduction can potentially mitigate assault rates.

---

## Project Structure
**Directory Tree:**

```bash
States-Grouping_Assault-Prediction/
│
├── README.md                                              # Project overview and instructions
├── States_Grouping_Assault_Prediction.md                  # Main analysis report
├── States_Grouping_Assault_Prediction.Rmd                 # Main analysis script
├── US_Arrest_Data/                                        # Data files (e.g., USArrest.csv, USstatex77.csv)
└── States-Grouping_Assault-Prediction_files/figure-gfm/   # Visuals used in the report
```

**Key Files:**
- **States_Grouping_Assault_Prediction.md:** The main Markdown report with analysis, viewable directly on GitHub.
- **States_Grouping_Assault_Prediction.Rmd:** The main R Markdown file containing the analysis.
- **US_Arrest_Data/:** Folder containing the input datasets.
- **States-Grouping_Assault-Prediction_files/figure-gfm/:** Folder to store generated outputs (e.g., reports, tables).

---

## License

This project is intended for submission as part of a technical assessment. The content and code are not intended for public distribution, reproduction, or commercial use without explicit permission from the Author.

---

## Contact Information

**Author:** Ou Yang Yu
