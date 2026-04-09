
# Faulty Medical Devices – Data Analysis

This project provides a structured analysis of faulty medical device event records. The objective was to develop a clear, end‑to‑end analytical workflow that cleans and standardises the raw data, merges multiple relational tables, and produces visual summaries that highlight reporting patterns across countries, notice types, and action types. The analysis is designed to support post‑market surveillance and quality improvement activities within regulated medical‑device environment

---

📊 Executive Summary
This analysis examines a multi‑table dataset containing event reports, device information, and manufacturer details. After conducting data cleaning and harmonisation, the merged dataset was used to explore trends in device‑related events, distribution of notice and action categories, and country‑level reporting behaviour.
The findings indicate that a small number of notice and action categories account for the majority of reported events, with reporting volume concentrated within specific countries. Year‑level trends show variation in annual reporting activity, and the visual outputs provide a consolidated view of the underlying patterns. These insights help stakeholders identify high‑volume categories, understand reporting consistency, and prioritise follow‑up activities.

---

## 📁 Project Structure

```text
faulty-medical-devices-analysis
│
├── README.md
├── notebooks/
│   └── analysis.ipynb
├── src/
│   └── clean_and_visualise.py
├── data/
│   └── README.md
└── outputs/
    └── charts/
```

---

📄 Data Context
The dataset consists of three linked tables:

Events – individual faulty device event records
Devices – device‑level metadata
Manufacturers – organisation details associated with each device

These tables required cleaning and normalisation, particularly for categorical fields that included inconsistent casing, punctuation, and duplicated category labels. The cleaned datasets were merged using matching IDs to create a consolidated analytical view.

---

## ✅ **Objective**

The aim of this analysis is to identify trends, high‑volume event types, and country‑level reporting patterns within faulty medical device events. By cleaning and standardising the dataset, then merging three related tables (events, devices and manufacturers), the goal is to produce insights that can inform quality teams, operational leads, and regulatory reporting.[1](https://github.com/leightonwilliams46-prog/nosql-data-analysis-tutorials/releases)

---

🔧 Methodology
The analysis followed these steps:


Data Cleaning

Standardised inconsistent text fields
Corrected category labels and harmonised naming
Removed formatting inconsistencies



Dataset Merging

Joined events, devices, and manufacturers to produce a single enriched dataset



Exploratory Analysis

Assessed event distribution across notice and action types
Reviewed country‑level reporting behaviour
Analysed multi‑year event trends



Visualisation

Created static visual outputs via Python
Exported charts to the /outputs/charts/ directory

---

## 📊 Key Visualisations

### Action Type Count
![Action Type Count](https://raw.githubusercontent.com/leightonwilliams46-prog/faulty-medical-devices-analysis/main/outputs/charts/action_type_count_clean.png)

The majority of events fall within two main action categories, indicating clear patterns in how issues are managed. This concentration suggests well‑established workflows for the most common event types.

### Events by Country
![Events by Country](https://raw.githubusercontent.com/leightonwilliams46-prog/faulty-medical-devices-analysis/main/outputs/charts/events_by_country.png)

Event reporting is highly concentrated, with several countries accounting for a disproportionate share of total events. This may reflect differences in regulatory reporting requirements, market size, or device utilisation volume.

### Events by Type
![Events by Type](https://raw.githubusercontent.com/leightonwilliams46-prog/faulty-medical-devices-analysis/main/outputs/charts/events_by_type.png)

A small number of notice types dominate the dataset. Understanding these categories helps identify systemic issues and prioritise root‑cause evaluations.

### Events by Year
![Events by Year](https://raw.githubusercontent.com/leightonwilliams46-prog/faulty-medical-devices-analysis/main/outputs/charts/events_by_year_CLEAN.png)

Event volume shows clear multi‑year trends. Peaks may align with regulatory changes, increased device distribution, or shifts in reporting practices. This time‑series view supports forecasting and helps contextualise sudden increases or declines.

---

📈 Insights & Interpretation
The analysis highlights several notable patterns:

Event reporting is dominated by a limited number of action types, indicating consistency in how most device issues are managed.
Notice types show similar concentration, suggesting that certain incident classes are more frequently encountered.
Country‑level reporting varies significantly, with some markets contributing disproportionately to overall volume.
Text‑field normalisation had a material impact on improving category accuracy and reducing duplicated labels.
The consolidated dataset provides a clearer view of device‑related issues and supports targeted quality review activities.

These observations can help quality, regulatory, and operational teams prioritise follow‑up actions and direct resources to high‑impact event categories.

---

🧪 How to Run the Analysis
To run this project locally:

Download the dataset files:

events-1681209680.csv
devices-1681209661.csv
manufacturers-1681209657.csv


Place them in the /data directory
Open notebooks/analysis.ipynb and run all cells
Alternatively, execute:
python src/clean_and_visualise.py

to generate visual outputs directly into /outputs/charts/.

---

🛠️ Tools & Libraries

Python: pandas, numpy, matplotlib, seaborn
Jupyter Notebook for exploratory analysis
Custom Python script for visual output generation
GitHub for version control and documentation

---

✅ Conclusion
This project demonstrates a complete analytical workflow for faulty medical device event data, covering cleaning, merging, visualisation, and high‑level interpretation. The insights help illustrate how event characteristics vary across categories, countries, and time, supporting more effective monitoring of post‑market device performance.
The structured approach, combined with automated visual outputs, provides a foundation for more advanced analytics such as trend forecasting, device‑category risk assessment, or integration into BI dashboards for operational reporting.

---

## ✅ **Next Steps**

If I extend this project, I’d like to:

- Add interactive charts (Plotly or Dash)  
- Build a simple Power BI or Tableau report using the cleaned output  
- Incorporate NLP to analyse free‑text event descriptions  
- Look at predictive modelling on event types or action categories  

---
