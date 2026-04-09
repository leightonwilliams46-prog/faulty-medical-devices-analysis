
# Faulty Medical Devices – Data Analysis

This project explores a historical dataset of faulty medical device event records. I wanted to build a clear, end‑to‑end analytical workflow that cleans the raw data, merges multiple tables, and produces visual summaries that help explain where issues occur and how reporting patterns change over time. The work is focused on supporting post‑market surveillance and quality improvement activities in regulated environments

---

## 📁 Project Structure

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

---

## ✅ **Objective**

The aim of this analysis is to identify trends, high‑volume event types, and country‑level reporting patterns within faulty medical device events. By cleaning and standardising the dataset, then merging three related tables (events, devices and manufacturers), the goal is to produce insights that can inform quality teams, operational leads, and regulatory reporting.[1](https://github.com/leightonwilliams46-prog/nosql-data-analysis-tutorials/releases)

---

## ✅ **What I Did**

This project covers:

- Cleaning and normalising inconsistent text fields  
- Merging event, device and manufacturer datasets  
- Exploring trends in faulty device reporting over time  
- Analysing the distribution of notice and action types  
- Identifying top reporting countries  
- Creating static visualisations to summarise key patterns[1](https://github.com/leightonwilliams46-prog/nosql-data-analysis-tutorials/releases)

---

## 📊 Key Visualisations

### Action Type Count
![Action Type Count](https://raw.githubusercontent.com/leightonwilliams46-prog/faulty-medical-devices-analysis/main/outputs/charts/action_type_count_clean.png)

### Events by Country
![Events by Country](https://raw.githubusercontent.com/leightonwilliams46-prog/faulty-medical-devices-analysis/main/outputs/charts/events_by_country.png)

### Events by Type
![Events by Type](https://raw.githubusercontent.com/leightonwilliams46-prog/faulty-medical-devices-analysis/main/outputs/charts/events_by_type.png)

### Events by Year
![Events by Year](https://raw.githubusercontent.com/leightonwilliams46-prog/faulty-medical-devices-analysis/main/outputs/charts/events_by_year_CLEAN.png)

---

## ✅ **Insights & Interpretation**

Here is a summary of the main things I observed from the dataset:

- A small number of action types account for most responses, with *Safety Notification* and *Recall* being the most common.  
- Event reporting increases noticeably in later years, suggesting either better surveillance or increased device usage.  
- Reporting is highly concentrated in a small set of countries, reflecting market size or regulatory practices.  
- Notice types follow a similar pattern, with a few categories dominating overall volume.  
- Text fields required standardisation due to inconsistent casing and duplicated categories — cleaning these had a major effect on the clarity of the final outputs.  

---

## ✅ **How to Run the Analysis**

To run this project locally:

1. Download the datasets used for development:  
   - `events-1681209680.csv`  
   - `devices-1681209661.csv`  
   - `manufacturers-1681209657.csv`  
2. Place them in the `/data` folder  
3. Open `notebooks/analysis.ipynb` and run all cells  
4. Alternatively, run `src/clean_and_visualise.py` to generate charts directly into `/outputs/charts/`

---

## ✅ **Tools & Libraries Used**

- Python (pandas, numpy, matplotlib, seaborn)  
- Jupyter Notebook  
- Custom Python script for automated cleaning and plotting  
- Git & GitHub for version control and documentation  

---

## ✅ **Why This Project Matters**

Faulty medical device events have real implications for patient safety, manufacturer obligations, and regulatory compliance. Understanding which devices fail, how often failures occur, and which actions are most common helps quality teams prioritise investigations and supports post‑market surveillance reporting.  

This project demonstrates my ability to take a messy operational dataset and turn it into something structured, analysed, and visually interpretable.

---

## ✅ **Next Steps**

If I extend this project, I’d like to:

- Add interactive charts (Plotly or Dash)  
- Build a simple Power BI or Tableau report using the cleaned output  
- Incorporate NLP to analyse free‑text event descriptions  
- Look at predictive modelling on event types or action categories  

---
