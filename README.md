# 📈 Marketing Mix Modeling with Google Meridian

This repository contains **two end-to-end MMM analyses** using simulated marketing datasets, leveraging **Google Meridian** to measure media impact, diagnose model fit, and optimize budget allocation.

---

## 📂 Notebooks Overview

### 1️⃣ **National-Level MMM** (`Google_Meridian_Simulated_Data_National.ipynb`)
**Dataset:** `Simulated_Data_National.csv`  
**Scope:**  
- Analyzes **national aggregated data** without geo breakdown.  
- Groups channels into:
  - 📊 **Impressions-based** (exposure counts)
  - 📡 **Reach/frequency-based** (audience breadth & repetition)
- Includes external factors such as `GQV`, `Geo_GDP`, and `Competitor_Discount`.

**Key Highlights:**
- 📉 **Seasonality & Trend Decomposition** of conversions.
- 🔍 **Correlation analysis** between media and KPIs.
- 🎯 **ROI estimation** for each channel.
- 🛠 **Budget optimization** to maximize conversions at fixed spend.

---

### 2️⃣ **Geo-Level MMM** (`Google_Meridian_Simulated_Data_RF.ipynb`)
**Dataset:** `Simulated_Data_RF.csv`  
**Scope:**  
- Runs MMM at **geo granularity**, with population, tier, and economic indicators.
- Captures **market heterogeneity** and competitive effects at regional level.

**Key Highlights:**
- 📍 **Geo-specific patterns** in impressions and spend.
- ⏱ **Lagged correlation** to measure immediate vs. delayed effects.
- 🧩 Inclusion of **geo controls** for competitive and economic conditions.
- 🛠 **Geo-level optimization** for targeted budget reallocation.

---

## 🛠 Workflow in Both Notebooks

1. **Data Preparation & Structuring**
   - Map raw data into **Meridian’s schema**.
   - Separate media variables into **conceptual groups**.
   - Add KPI, revenue, and control variables.

2. **Exploratory Analysis**
   - Time trends, correlations, and lag effects.
   - Identify seasonal patterns and variance.

3. **Model Specification**
   - Use **data-guided priors** (log-normal ROI priors).
   - Configure adstock & saturation curves.

4. **Model Fitting & Diagnostics**
   - Check **R-hat** convergence.
   - Compare **predicted vs. actual** KPIs.

5. **Results & Insights**
   - Channel ROI and contribution analysis.
   - Baseline vs. media-driven KPI lift.

6. **Budget Optimization**
   - Recommend optimal spend allocation.
   - Estimate potential KPI lift.

---

## 📊 Outputs & Visuals
Both notebooks produce:
- ✅ Convergence diagnostics (R-hat plots)
- ✅ Expected vs. actual KPI charts
- ✅ Channel contribution and ROI tables
- ✅ Optimization recommendations

---

🧠 Intended Audience
Non-technical stakeholders: Focus on plots, summaries, and recommendations.

Analysts & Data Scientists: Review code cells, model specs, and diagnostics for methodology details.

Marketers & Strategists: Use ROI and optimization outputs for campaign planning.

---
📌 Notes
Data is simulated for demonstration purposes.

The methods and structure are aligned with Google Meridian MMM workflows.
