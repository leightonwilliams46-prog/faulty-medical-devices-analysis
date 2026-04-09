
# Faulty Medical Devices – Data Analysis

This project explores a dataset of faulty medical device event records.  
The work covers data cleaning, text normalisation, table merging, visualisation and interpretation, with a focus on supporting post‑market surveillance activities.

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

## 🔍 About This Project

The analysis examines:

- Trends in reported events over time  
- Most frequent notice and action types  
- Country‑level reporting patterns  
- Cleaning and normalisation of inconsistent text fields  
- Merging of event, device and manufacturer datasets  

The notebook provides a step‑by‑step walk‑through of the analytical workflow, while the Python script generates a set of static visualisations.

---

## 🚀 Running the Notebook

To run the analysis locally:

1. Download the dataset files used during development:
   - `events-1681209680.csv`
   - `devices-1681209661.csv`
   - `manufacturers-1681209657.csv`
2. Place them inside the `/data` folder.
3. Open `notebooks/analysis.ipynb` and run all cells.

The script `clean_and_visualise.py` uses the same files and will save charts into the `/outputs/charts` directory when executed.

---

## 📊 Key Visualisations

![Action Type Count](https://raw.githubusercontent.com/leightonwilliams46-prog/faulty-medical-devices-analysis/main/outputs/charts/action_type_count_clean.png)

### Events by Country
https://raw.githubusercontent.com/leightonwilliams46-prog/faulty-medical-devices-analysis/main/outputs/charts/events_by_country.png

### Events by Type
https://raw.githubusercontent.com/leightonwilliams46-prog/faulty-medical-devices-analysis/main/outputs/charts/events_by_type.png

### Events by Year
https://raw.githubusercontent.com/leightonwilliams46-prog/faulty-medical-devices-analysis/main/outputs/charts/events_by_year_CLEAN.png

---

## 📊 Visual Outputs

Charts generated during the analysis can be found in:

outputs/charts/

These include:

- Events over time  
- Notice type distribution  
- Action type frequency  
- Top reporting countries  

---

## 📝 Summary

The project demonstrates a complete end‑to‑end data analysis workflow using Python, including cleaning a large dataset, merging multiple tables, producing visualisations and summarising findings relevant to medical device post‑market surveillance.
