# 🌍 AI-Driven CO₂ Emissions Analysis

End-to-end analysis of global CO₂ emissions, electricity carbon intensity, and top emitting countries using public datasets from Our World in Data (OWID). The goal is to understand how regional energy grids impact the carbon footprint of AI and cloud workloads and to propose data-driven sustainability strategies.

---

## 📌 Overview

- Analyze long-term global CO₂ emission trends  
- Build a 5-year emission projection using Linear Regression  
- Compare electricity carbon intensity (India vs US vs World)  
- Identify top CO₂-emitting countries  
- Convert insights into clear, actionable recommendations  

This project was created as part of a **Data Analyst assignment for Antarctica Global** and also serves as a portfolio project in **data analytics + sustainability**.

---

## 📂 Datasets

**1. Global CO₂ Emissions (OWID)**  
- ~60,000 rows  
- Fields: `country`, `iso_code`, `year`, `co2`  
- Cleaned by removing aggregate regions and keeping real countries only  

**2. Carbon Intensity of Electricity (OWID)**  
- ~5,700 rows  
- Fields: `entity`, `year`, `carbon_intensity`  
- Filtered for India, United States, and World; missing values removed  

---

## 🛠 Tech Stack

- Python, Jupyter Notebook  
- Pandas, NumPy  
- Matplotlib  
- Scikit-learn (LinearRegression)  

---

## 📈 Main Visualizations

1. Global CO₂ Emissions Trend (1990–Present)  
2. 5-Year CO₂ Emission Projection  
3. Electricity Carbon Intensity by Region (India vs US vs World)  
4. Top 5 CO₂ Emitting Countries (latest year)  

Each chart includes short, focused insights.

---

## 🧠 Key Insights (Summary)

- Global CO₂ emissions have steadily increased since 1990, with only small temporary dips.  
- Linear Regression projection shows emissions continuing to rise in the near future.  
- India’s grid is far more carbon-intensive (~708 gCO₂/kWh) than the US (~383 gCO₂/kWh) and the global average.  
- China, the US, India, Russia and Japan are the top CO₂ emitters globally.  

---

## ♻️ Strategic Recommendations (Short)

1. **Run workloads in low-carbon regions** (US/EU instead of high-intensity regions like India).  
2. **Optimize AI training** via fine-tuning, smaller models, pruning, quantization, and early stopping.  
3. **Prefer cloud providers with strong renewable energy commitments** and carbon-free energy matching.  
4. **Use carbon-aware scheduling** to run non-urgent jobs during low-carbon hours (solar/wind peaks).  
5. **Improve hardware lifecycle** by extending server/GPU lifespan and optimizing cooling.  
6. **Track IT emissions** using CO₂ budgets, dashboards and FinOps/GreenOps-style governance.

---

## 📁 Project Structure

- `Antarctica-Global-CO2-Emissions-Analysis.ipynb` – main analysis notebook  
- `Report.pdf` – 4-page structured report (intro, analysis, visuals, recommendations)  
- `README.md` – this documentation  

---

## ▶️ How to Run

1. Clone the repository  
2. Download OWID datasets and save as:
   - `owid-co2-data.csv`
   - `carbon-intensity-electricity.csv`
3. Open the notebook:
   ```bash
   jupyter notebook Antarctica-Global-CO2-Emissions-Analysis.ipynb
