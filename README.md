# COVID-19 Data Analysis: Uncovering Key Trends and Insights in India 📊

## Overview

This project explores the impact of COVID-19 in India through **data cleaning, exploratory analysis, and visualizations**. Using the global OWID COVID-19 dataset, the analysis focuses on identifying key patterns in case progression, deaths, testing, vaccinations, and socio-economic factors that influenced outcomes.

The goal is to **uncover meaningful insights** into how the pandemic evolved in India and to assess the effectiveness of intervention measures and healthcare capacity.

## Dataset Details

The dataset is provided by **Our World in Data (OWID)** and includes daily COVID-19 records for countries worldwide.

### Key Columns Analyzed

* **Cases & Deaths:** `total_cases`, `new_cases`, `total_deaths`, `new_deaths`
* **Testing & Positivity:** `total_tests`, `new_tests`, `positive_rate`
* **Vaccinations:** `total_vaccinations`, `people_vaccinated`, `people_fully_vaccinated`
* **Healthcare Capacity:** `icu_patients`, `hosp_patients`, `hospital_beds_per_thousand`
* **Government Measures:** `stringency_index`
* **Socio-Economic Indicators:** `gdp_per_capita`, `median_age`, `aged_65_older`, `diabetes_prevalence`, `extreme_poverty`, `life_expectancy`, `human_development_index`

Dataset source: [OWID COVID-19 Data](https://www.kaggle.com/datasets/hosammhmdali/covid-19-dataset)

## Project Workflow

### 1. Data Cleaning & Preprocessing

* Handled missing values across cases, deaths, testing, and vaccination columns.
* Replaced missing socio-economic indicators with country-specific medians.
* Converted `date` column to datetime format.
* Retained outliers (e.g., spikes in cases/deaths) as they represent real-world events.

### 2. Exploratory Data Analysis (EDA)

* Summarized data structure, shape, and key statistics.
* Isolated **India’s data (`df_india`)** for focused analysis.
* Derived new metrics such as **Case Fatality Rate (CFR)**, **recovery rate**, **positivity rate**, and **active cases**.

### 3. Data Visualization

Created impactful visualizations using **Matplotlib** and **Seaborn**, including:

* **Time-series plots** for new cases, new deaths, vaccination progress, and active cases.
* **Scatter plots** for testing vs. cases, hospital beds vs. deaths, smoking rates vs. deaths, and diabetes prevalence vs. cases.
* **Boxplots & heatmaps** to compare extreme poverty and socio-economic indicators against outcomes.
* **Proportional plots** for new cases relative to population size.

### 4. Analytical Questions Answered

* When were the **first and last reported cases** in India?
* What were the **highest daily counts** of new cases, deaths, and vaccinations?
* What are the **total cases, deaths, CFR, and recovery rate** in India?
* How did **vaccination and testing trends** influence case detection?
* What socio-economic factors (age, poverty, smoking, diabetes, healthcare capacity) correlated with COVID-19 outcomes?

## Key Insights

* **Peak Outbreaks:** India recorded its highest surge of daily cases and deaths during the 2nd wave (Delta variant).
* **Vaccination:** Significant ramp-up in 2021–2022, with over **60% of the population fully vaccinated**.
* **Testing & Positivity:** More testing correlated with higher case detection, while positivity spikes aligned with major waves.
* **Healthcare Capacity:** Limited hospital beds per thousand correlated with high mortality during outbreak peaks.
* **Demographics:** Higher elderly population and co-morbidities (e.g., diabetes) increased vulnerability.
* **Government Measures:** Periods of strict interventions (lockdowns, stringency index spikes) coincided with declines in new cases.

## Why This Matters

This analysis provides **evidence-based insights** into India’s COVID-19 response:

* **Public health officials** can assess which measures were most effective.
* **Researchers** gain perspective on socio-economic vulnerabilities.
* **Data scientists** see how real-world crises can be analyzed with Python tools.

## Jupyter Notebook

The complete workflow, analysis, and visualizations are available in this repository.
