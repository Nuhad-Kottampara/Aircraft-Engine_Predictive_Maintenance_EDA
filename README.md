**Multi-Sensor Analysis for Aircraft Engine Predictive Maintenance**

✈️ **Project Overview**
This project performs an end-to-end Exploratory Data Analysis (EDA) on the NASA CMAPSS (Commercial Modular Aero-Propulsion System Simulation) dataset. The goal is to identify mechanical degradation patterns in turbofan engines through sensor data analysis, enabling a transition from reactive to Condition-Based Maintenance (CBM) strategies.

🛠️ **Technical Stac**k

Language: Python 3.x

Libraries: Pandas, NumPy, Matplotlib, Seaborn

Environment: Jupyter Notebook / Google Colab

📂 **Dataset Description**

The dataset consists of multiple multivariate time-series. Each engine starts with normal variations but develops a fault over time until operational failure.

Key Features analyzed: s4 (LPT Outlet Temp), s11 (HPC Outlet Pressure), s12 (Fuel Flow Ratio), and s15 (Bypass Ratio).

Derived Feature: engine_stage (Categorizing cycles into 'Healthy', 'Operating', and 'Failing').

📊 **Key Analysis & Visualizations**

The project includes over 10 distinct visualizations covering:

Univariate Analysis: Histograms and Box Plots to identify data distribution and outliers in failing engines.

Bivariate Analysis: Line charts showing sensor trends over operational cycles and a Correlation Heatmap to identify redundant signals.

Multivariate Analysis: Colorblind-friendly pairplots to visualize the "failure cluster" where temperature and pressure interact.

💡 **Key Insights**

Primary Indicators: Sensors s4 and s11 are the most reliable predictors, showing a sharp upward trend ~30 cycles before failure.

Thermal-Pneumatic Collapse: A near-perfect correlation exists between core temperature and pressure, indicating systemic engine degradation.

Outlier Significance: High-side outliers are not errors; they represent engines entering a high-risk pre-failure state.

Efficiency Loss: Significant instability in fuel flow ratios (s12) occurs in the final stages of engine life.

Maintenance Strategy: The variance in engine lifespans (128 to 300+ cycles) proves that sensor-driven maintenance is far more efficient than fixed-schedule maintenance.

🚀 **Future Work**

Machine Learning: Building a regression model to predict Remaining Useful Life (RUL).

Feature Engineering: Implementing rolling averages to smooth sensor noise.

Deployment: Creating a real-time monitoring dashboard for fleet management.

👤 **Author**

Nuhad Kottampara 
Data Analytics Project - January 2025
