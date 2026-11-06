# Unemployment Analysis with Python

A data analysis project exploring unemployment trends across Indian regions using Python, Pandas, Matplotlib, and Seaborn.

## Project Overview

This project analyses unemployment data across 28 Indian regions from May 2019 to June 2020. It explores regional differences, monthly trends, relationships between employment indicators, and changes observed during the COVID-19 period.

The project was completed as part of the Oasis Infobyte Data Science Internship.

## Objectives

- Analyse unemployment rates across Indian regions.
- Explore monthly unemployment trends.
- Compare unemployment patterns across selected regions.
- Identify the ten regions with the highest average unemployment rates.
- Examine correlations between employment indicators.
- Compare average unemployment before and after the COVID-19 lockdown boundary.

## Technologies Used

- Python 3
- Jupyter Notebook
- Pandas
- NumPy
- Matplotlib
- Seaborn

## Dataset

**Primary dataset:** `Unemployment in India.csv`

The dataset contains the following fields:

- Region
- Date
- Frequency
- Estimated Unemployment Rate (%)
- Estimated Employed
- Estimated Labour Participation Rate (%)
- Area

The original dataset contained 768 rows. After removing 28 completely empty rows and converting the date column, 740 valid observations remained.

No additional duplicate observations were found after removing the empty rows.

## Project Workflow

1. Dataset loading and inspection.
2. Data quality assessment.
3. Removal of completely empty records.
4. Date conversion and data type verification.
5. Exploratory data analysis.
6. Regional unemployment analysis.
7. Monthly trend visualisation.
8. Comparison of three selected regions.
9. Identification of the top ten regions.
10. Correlation analysis.
11. Pre-COVID and post-COVID comparison.
12. Findings and conclusions.

## Key Findings

- Overall average unemployment rate: **11.79%**.
- Number of regions analysed: **28**.
- Tripura recorded the highest average regional unemployment rate.
- Meghalaya recorded the lowest average regional unemployment rate.
- Unemployment increased sharply during April and May 2020 in the overall monthly trend.
- Jharkhand recorded a particularly high unemployment peak among the three selected regions.
- Correlation between unemployment rate and estimated employment: **-0.22**.
- Correlation between unemployment rate and labour participation rate: **0.00**.
- Pre-COVID average unemployment rate: **9.51%**.
- Post-COVID average unemployment rate: **17.77%**.
- Difference between the two averages: **8.26 percentage points**.

## COVID-19 Comparison Method

The analysis uses 25 March 2020 as the comparison boundary.

- Pre-COVID: observations dated before 25 March 2020.
- Post-COVID: observations dated on or after 25 March 2020.

The comparison is descriptive and does not independently establish causation.

## Project Structure

```text
DataScience-Task2-UnemploymentAnalysis/
│
├── data/
│   ├── raw/
│   │   ├── Unemployment in India.csv
│   │   └── Unemployment_Rate_upto_11_2020.csv
│   │
│   └── processed/
│
├── Screenshots/
│
├── Unemployment_Analysis.ipynb
├── README.md
├── requirements.txt
└── .gitignore
```

The virtual environment is excluded from version control.

## How to Run

1. Clone the repository.
2. Open the Task 2 project folder.
3. Create and activate a Python virtual environment.
4. Install the dependencies:

```bash
pip install -r requirements.txt
```

5. Open `Unemployment_Analysis.ipynb` in Jupyter Notebook or VS Code.
6. Select the appropriate Python kernel.
7. Run all notebook cells.

## Limitations

- The dataset covers May 2019 to June 2020 only.
- The post-COVID comparison period contains fewer observations.
- Regional averages combine Rural and Urban observations.
- Correlation does not establish causation.
- The findings describe the supplied historical dataset and should not be interpreted as current unemployment statistics.

## Conclusion

This project demonstrates how Python-based exploratory data analysis and visualisation can reveal regional differences, historical trends, and relationships between employment indicators.

The analysis identified substantial changes in unemployment during the period covered by the dataset, particularly around the COVID-19 lockdown period.

---

**Internship:** Oasis Infobyte  
**Track:** Data Science  
**Project:** Unemployment Analysis with Python