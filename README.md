# 💡 Python Project by Yash Yennewar

# 🌍 Global_Warming_Data_Analysis_Project
This project explores global warming trends using a dataset of climate-related indicators across countries and years (1900–2023).  

## 🔗 Project Link :

[Global_Warming_Data_Analysis](Global_Warming_Data_Analysis.ipynb)

---

## 📌 Project Overview :
The notebook analyzes how **CO₂ emissions, methane emissions, temperature anomalies, Arctic ice extent, and air pollution** vary over time and across regions.
The analysis includes:
- Data cleaning & preprocessing  
- Descriptive statistics  
- Visualizations (trends, boxplots, histograms)  
- Country-level comparisons  
- Insights into climate change indicators  

---

## 🛠️ Tools Used :
The analysis and visualization were performed using the following Python libraries:
- Pandas – for data manipulation and analysis
- Seaborn – for statistical data visualization
- Matplotlib – for plotting and data visualization

---

## 📂 Dataset :
The dataset consists of the following files:
- Dataset Source : [Global_Warming Dataset](https://www.kaggle.com/datasets/ankushpanday1/global-warming-dataset-195-countries-1900-2023)

---

## 📂 Repository Structure :
```bash
├── Global_Warming_Data_Analysis.ipynb   # Jupyter Notebook with analysis
├── data/                                # (Optional) Place dataset here
├── README.md                            # Project documentation
└── requirements.txt                     # Python dependencies
```
---

## 📊 Key Features :
- Trend Analysis: Global and country-level climate indicators over 1900–2023.
- Visualization: Line plots, histograms, and boxplots for emission and temperature patterns.
- Country Comparison: Compare emissions, air pollution, and ice extent across nations.
- Statistical Insights: Descriptive stats and distribution analysis.

---

## 💡Final Insights :
1. Large synthetic-like dataset with wide ranges — The variables show broad ranges (CO₂, methane, population, GDP in other columns).The Temperature_Anomaly range (≈ −2 to +2) + the tidy quantiles suggest this dataset is likely synthetic or normalized for demo/education (not raw real-world units).Treat absolute numbers cautiously if you intend to make real-world claims.<br><br>
2. CO₂ and methane are large and skewed — Means are high and distributions have long tails (stds are large compared to means).Expect right skew / heavy-tail behavior; boxplots and histograms in the notebook confirm this.<br><br>
3. Arctic ice extent distribution — Mean ≈ 8 with wide spread and long tails (min ≈ 1, max ≈ 15).The histograms and time-series plots in the notebook indicate strong temporal behavior — likely a downward long-term trend (the notebook plotted Arctic_Ice_Extent trend).<br><br>
4. Air pollution is variable — Mean ≈ 149 but large standard deviation; some countries/years have very low index values while others are very high (up to ≈ 300).Country-level boxplots in the notebook show clear between-country variation.<br><br>
5. Temperature anomaly centered near zero — Mean near zero with ±2 range; but the trend matters more than the mean.Notebook contains lineplots for time-series variables (CO₂, methane, Arctic ice, etc.) — these visualizations are the correct approach to detect long-term trends.<br><br>
6. Country-level heterogeneity — Boxplots grouped by country (the notebook does this for the first 10 countries) show big between-country differences across variables — good candidate for clustering countries into groups (e.g., high emissions / low emissions / high pollution / low pollution).
</div><br><br>
Limitations & cautions<br><br>
1. Likely synthetic / scaled data — some columns (e.g., Temperature_Anomaly bounded at ±2, CO₂ rounded near 1e9) suggest generated values. If your aim is real-world inference, validate and replace with authoritative datasets (e.g., NOAA, CDIAC, GISS, NASA, WMO, EPA).<br><br>
2. Units not explicit — many variables lack unit labels in the notebook (e.g., CO₂ units, Arctic ice units). Add explicit units in plots and table captions.<br><br>
3. Temporal aggregation and autocorrelation — time-series analysis must account for temporal autocorrelation before doing standard regression or correlation tests.<br><br>
4. Missing real-world metadata — country codes, region, income group would help group analysis and policy-relevance.

---
