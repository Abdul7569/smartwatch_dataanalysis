# Smartwatch Health Data Cleaning and Analysis

This repository contains a Jupyter Notebook (`smartwatch_health_data_analysis.ipynb`) that processes and analyzes an unclean dataset of smartwatch health metrics. The project demonstrates data cleaning techniques using Pandas and visualizes relationships between health metrics (e.g., heart rate and stress levels) using Seaborn and Matplotlib.

## Project Overview

The dataset (`unclean_smartwatch_health_data.csv`) includes health metrics such as User ID, Heart Rate (BPM), Blood Oxygen Level (%), Step Count, Sleep Duration (hours), Activity Level, and Stress Level. The notebook:
1. Loads and inspects the raw data.
2. Handles missing values and data type inconsistencies.
3. Identifies outliers in numerical columns.
4. Visualizes the relationship between Heart Rate and Stress Level using a binned boxplot.

This project is ideal for learning basic data cleaning, exploratory data analysis (EDA), and visualization in Python.

## Dataset

- **File:** `unclean_smartwatch_health_data.csv` (not included in the repository due to size/privacy; sample output shown in notebook)
- **Columns:**
  - `User ID` (float64): Unique identifier for users
  - `Heart Rate (BPM)` (float64): Heart rate in beats per minute
  - `Blood Oxygen Level (%)` (float64): Blood oxygen saturation percentage
  - `Step Count` (float64): Daily step count
  - `Sleep Duration (hours)` (object, converted to float64): Hours slept
  - `Activity Level` (object): Categorical (e.g., "Highly Active", "Sedentary")
  - `Stress Level` (object, converted to float64): Stress score (1-10)

- **Issues:** Missing values (NaN), inconsistent data types (e.g., "ERROR" in Sleep Duration), typos in categorical data (e.g., "Seddentary"), and outliers (e.g., Heart Rate of 247 BPM).

## Prerequisites

To run this notebook, you need the following installed:
- Python 3.9+ (tested with 3.9.21)
- Jupyter Notebook or JupyterLab
- Required Python libraries:
  - `pandas`
  - `seaborn`
  - `matplotlib`

### Installation

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/[your-username]/smartwatch-health-data-analysis.git
   cd smartwatch-health-data-analysis
