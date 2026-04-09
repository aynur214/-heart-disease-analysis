Heart Disease Data Analysis | Python EDA + Power BI Dashboard

Project Overview
This project presents an end-to-end Exploratory Data Analysis (EDA) of the UCI Heart Disease dataset to identify patterns and key factors associated with heart disease. 
The results are visualized through an interactive Power BI dashboard and are descriptive in nature, meaning they should not be used for clinical decision-making.

## Problem Statement
Medical professionals deal with large volumes of patient data daily. 
Without proper visualization and analysis, identifying patterns in this 
data is time-consuming and error-prone. This project demonstrates how 
data analysis tools can help surface meaningful patterns from clinical data.

## Solution
Using Python for EDA and Power BI for interactive visualization, this 
project transforms raw patient data into clear, structured insights. 
The dashboard allows users to explore the data interactively — filtering 
by gender, age range, and disease status to compare patient profiles.

## Tools & Technologies
- **Python** — Data manipulation and visualization
  - `Pandas` — Data loading, cleaning, and analysis
  - `NumPy` — Numerical computations
  - `Matplotlib` — Basic visualizations
  - `Seaborn` — Statistical visualizations (heatmap, boxplot, scatter)
- **Power BI Desktop** — Interactive dashboard
- **Google Colab** — Cloud-based development environment
- **Git & GitHub** — Version control and portfolio hosting
## Dataset
| Property | Value |
|---|---|
| Source | UCI Machine Learning Repository |
| Patients | 303 |
| Features | 14 |
| Missing Values | None |
| Target Variable | Heart Disease (1=Yes, 0=No) |

## Feature Descriptions
| Column | Description |
|---|---|
| `age` | Age of the patient (29–77 years) |
| `sex` | Gender (1=Male, 0=Female) |
| `cp` | Chest pain type (0=Typical angina, 3=Asymptomatic) |
| `trestbps` | Resting blood pressure (mmHg) |
| `chol` | Serum cholesterol (mg/dL) |
| `fbs` | Fasting blood sugar > 120 mg/dL (1=True, 0=False) |
| `restecg` | Resting ECG results (0=Normal, 1=Abnormal) |
| `thalach` | Maximum heart rate achieved |
| `exang` | Exercise induced angina (1=Yes, 0=No) |
| `oldpeak` | ST depression induced by exercise |
| `slope` | Slope of peak exercise ST segment |
| `ca` | Number of major vessels colored by fluoroscopy (0–4) |
| `thal` | Thalassemia type |
| `target` | Heart disease presence (1=Yes, 0=No) |

---
## Project Steps

### 1 — Data Collection
Loaded the UCI Heart Disease dataset directly from GitHub using Pandas.

### 2 — Data Exploration
Examined dataset structure, data types, and basic statistics.
Confirmed: 303 rows, 14 columns, no missing values.

### 3 — Statistical Analysis
Performed descriptive statistics to understand distributions.
- Average age: 54.4 years
- Average cholesterol: 246 mg/dL
- 54.5% of patients in the dataset have heart disease

### 4 — Data Visualization
Created 4 visualizations:
- **Age Distribution** — Age patterns by disease status
- **Gender Analysis** — Disease rates by gender
- **Cholesterol Distribution** — Boxplot comparison between groups
- **Age vs Max Heart Rate** — Scatter plot showing relationship

### 5 — Correlation Analysis
Built a heatmap to identify features most strongly associated with 
heart disease. Note: correlation does not imply causation.

### 6 — Power BI Dashboard
Built an interactive dashboard with 4 visualizations. Users can filter 
by gender and disease status to explore patient profiles and compare groups.

---
## Key Findings & Conclusion

The following findings are based on this specific dataset (303 patients) 
and should be interpreted with caution:

- **54.5%** of patients in this dataset have heart disease (165 out of 303)
- **Female patients show a higher disease rate (75%)** compared to males (45%) 
  in this sample — this may reflect sample composition rather than 
  real-world population patterns
- **Chest pain type** shows the strongest positive association with heart 
  disease (correlation: +0.43)
- **Exercise-induced angina** is strongly associated with disease presence 
  (correlation: -0.44)
- **Cholesterol** shows very weak association with disease in this dataset 
  (correlation: -0.09) — this is a notable finding worth further investigation
- **Maximum heart rate** is negatively associated with disease 
  (correlation: +0.42), suggesting patients with disease tend to have 
  lower maximum heart rates
- Most patients with heart disease fall in the **40–55 age range** in this dataset



