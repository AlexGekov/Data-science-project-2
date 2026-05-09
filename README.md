# 🌍 Global Life Expectancy Analysis: The Impact of Macroeconomic and Environmental Factors

![Python Version](https://img.shields.io/badge/python-3.8%2B-blue.svg)
![Jupyter Notebook](https://img.shields.io/badge/tools-Jupyter-orange.svg)
![Libraries](https://img.shields.io/badge/libraries-pandas%20%7C%20scikit--learn%20%7C%20seaborn-green.svg)

## 📌 Project Overview
This repository contains a complete, end-to-end data science project analyzing the complex relationship between a nation's life expectancy, its macroeconomic prosperity, and its environmental degradation. 

The primary objective is to investigate how factors like **GDP per capita** and **PM2.5 Air Pollution exposure** influence public health outcomes on a global scale. By merging and analyzing distinct datasets, this project translates real-world health and economic challenges into a rigorous mathematical and statistical framework.

## 📊 Data Sources
This analysis relies on combining and cross-validating data from two independent, highly reputable sources:
1. **World Health Organization (WHO):** Life Expectancy and Adult Mortality data across various nations. ([Source Link](https://www.kaggle.com/datasets/kumarajarshi/life-expectancy-who))
2. **The World Bank:** Global Economic (GDP per capita) and Environmental (PM2.5 exposure) indicators. 
(Source Links:(https://data.worldbank.org/indicator/NY.GDP.PCAP.CD), (https://data.worldbank.org/indicator/EN.ATM.PM25.MC.M3))

## ⚙️ Methodology
This project follows a structured data science lifecycle:
* **Data Engineering:** Consolidating independent datasets, handling missing values, and standardizing nomenclature.
* **Exploratory Data Analysis (EDA):** Utilizing univariate and bivariate analysis to identify distributions, outliers, and underlying correlations.
* **Statistical Rigor:** Applying hypothesis testing (e.g., independent t-tests) to validate the statistical significance of environmental impacts on health.
* **Machine Learning & Mathematical Modeling:** * Implementing a baseline **Multiple Linear Regression** model.
  * Utilizing an advanced **Random Forest Regressor** to capture non-linear interactions.
  * Evaluating models using standard metrics (MAE, MSE, $R^2$).

## 📁 Repository Structure
```text
├── data/
│   ├── raw/                      # Original, immutable datasets (CSV)
│   └── processed/                # Cleaned and merged data (generated via code)
├── analysis.ipynb                # Main Jupyter Notebook with code, math, and text
├── .gitignore                    # Ignored files and cache directories
└── README.md                     # Project documentation
```

## 📈 Key Findings
* **Economic Impact:** A strong positive/logarithmic correlation was observed between GDP per capita and life expectancy.
* **Environmental Impact:** An independent T-test confirmed that PM2.5 pollution has a statistically significant negative impact on average lifespans.
* **Model Performance:** The Random Forest Regressor vastly outperformed the baseline Linear model, yielding an $R^2$ of **0.9595** and an MAE of **1.26 years**, highlighting the non-linear nature of global health metrics.
