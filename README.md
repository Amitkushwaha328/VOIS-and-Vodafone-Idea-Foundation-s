# 🌾 Seasonal Agriculture Performance Analysis

Major Project | VOIS AICTE Batch1 2026–2027 | Data Analytics

## 📌 Overview

This project analyzes agricultural performance across three farming seasons — **Kharif, Rabi, and Zaid** — using a dataset of 4,000 farm records spanning multiple Indian states, districts, and crops. It investigates how environmental conditions, resource usage, and economic outcomes vary seasonally, and identifies the key drivers behind those differences using statistical testing and machine learning.

## ❓ Problem Statement

Agricultural activities are influenced by seasonal variations in environmental conditions, farming practices, resource availability, and market conditions. Raw agricultural data alone does not clearly reveal how performance changes across seasons. This project analyzes the dataset to uncover meaningful seasonal patterns, trends, relationships, and variations.

## 🎯 Objectives

- Explore and clean the seasonal agriculture dataset
- Compare crop yield, cost, revenue, and profitability across seasons
- Examine how environmental factors (rainfall, temperature, humidity, soil moisture) affect performance
- Analyze resource usage (irrigation, fertilizer, water) by season
- Test statistical significance of seasonal differences (ANOVA)
- Identify key yield drivers using a Random Forest model
- Derive evidence-based recommendations for stakeholders

## 📂 Dataset

- **Records:** 4,000 farm entries
- **Features:** 34 columns including `State`, `District`, `Crop`, `Season`, `Rainfall_mm`, `Avg_Temperature_C`, `Humidity_pct`, `Soil_Moisture_pct`, `Nitrogen/Phosphorus/Potassium_kg_ha`, `Yield_Tonnes_Ha`, `Production_Tonnes`, `Total_Cost_INR`, `Revenue_INR`, `Profit_INR`, `ROI_pct`, `Water_Used_m3`, `Disease_Pest_Risk_pct`, and more.

## 🛠️ Technology Used

| Category | Tools |
|---|---|
| Language | Python 3 |
| Data Handling | Pandas, NumPy |
| Visualization | Matplotlib, Seaborn |
| Statistical Testing | SciPy (One-Way ANOVA, Kruskal-Wallis) |
| Machine Learning | Scikit-learn (Random Forest Regressor) |
| Environment | Jupyter Notebook |

## 🧪 Methodology

1. **Data Cleaning & Feature Engineering** — handled missing values; engineered `Cost_Per_Hectare`, `Revenue_Per_Hectare`, `NPK_Total`, `Is_Profitable`
2. **Exploratory Data Analysis** — seasonal comparisons via bar plots, violin plots, and correlation heatmaps
3. **Statistical Testing** — One-Way ANOVA on Yield, ROI, Rainfall, and Disease/Pest Risk across seasons
4. **Machine Learning** — Random Forest Regressor to rank feature importance for yield prediction
5. **Insight Synthesis** — translated findings into actionable recommendations

## 📊 Key Findings

- **ROI, Rainfall, and Disease/Pest Risk** vary significantly across seasons (ANOVA p < 0.05); Yield differences were **not** statistically significant
- **Rabi season** shows the highest consistency, profitability, and lowest risk
- **Kharif season** has the highest disease/pest risk, driven by high humidity and rainfall
- **Zaid season** relies heavily on artificial irrigation due to low natural rainfall
- **Seed Quality Score** and **Crop type** are stronger yield predictors than marginal fertilizer increases (Random Forest feature importance)

## 💡 Recommendations

1. Prioritize certified seed quality programs over blanket fertilizer subsidies
2. Deploy early-warning pest forecasting systems for Kharif season
3. Promote micro-irrigation (drip/sprinkler) adoption in Zaid season
4. Expand acreage under high-value, low-risk Rabi crops

## 🚀 Future Scope

- Time-series forecasting for next-season yield and ROI prediction
- Integration of satellite/NDVI data for real-time crop health monitoring
- District-level interactive dashboard for policymakers
- Incorporating market price volatility for stronger economic modeling
- Benchmarking against XGBoost / Gradient Boosting models

## 📁 Repository Structure

```
├── Seasonal_Agriculture_Analysis.ipynb   # Full analysis notebook
├── data/                                 # Dataset (if included)
├── README.md                             # Project documentation
└── VOIS_Major_Project_PPT_Submission.pptx # Presentation slides
```

## ▶️ How to Run

```bash
pip install pandas numpy matplotlib seaborn scipy scikit-learn
jupyter notebook Seasonal_Agriculture_Analysis.ipynb
```

## 👤 Author

**Amit Rajendra Kushwaha**
VOIS AICTE Batch1 2026–2027

## 📄 License

This project is submitted as part of the VOIS AICTE Major Project requirements.
