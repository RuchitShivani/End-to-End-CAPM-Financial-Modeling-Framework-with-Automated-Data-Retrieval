# Automated CAPM-Based Financial Analysis System Using Python

This project implements a fully automated **Capital Asset Pricing Model (CAPM)** analytics pipeline that fetches stock market data, computes daily returns, estimates beta and alpha, generates CAPM expected returns, produces interactive visualizations, and exports all results into an Excel workbook.

The repository includes **sample outputs (graphs + Excel)** generated from a **comparison of AAPL vs HBI vs TSLA**, demonstrating how the system works with real-world data.

---

## 🚀 Features

### ✔ Automated Data Retrieval
- Fetches historical stock price data from **Yahoo Finance**.
- Automatically retrieves **S&P 500 (SP500)** to use as the **market benchmark**.

### ✔ Complete End-to-End CAPM Pipeline
Includes:
1. Data fetching  
2. Data cleaning & normalization  
3. Daily returns calculation  
4. Beta & alpha estimation using regression  
5. CAPM expected return computation  
6. Interactive graph generation (Plotly)  
7. Automatic Excel report creation  
8. Auto-download support for Google Colab  

### ✔ Smart Visualization System
- Raw Price Chart  
- Normalized Price Chart (recommended for comparisons)  
- Automatic **scale distortion detection**  
- Secondary-axis graph when one ticker dominates the scale  
- Stock vs. market scatterplots with regression lines for beta estimation  

📌 **Note:**  
The graphs and Excel report uploaded in this repository come from a **sample CAPM comparison of AAPL, HBI, and TSLA**.

### ✔ Excel Report (Power BI Ready)
The script generates **capm_output.xlsx** with sheets:
- `Prices`  
- `Normalized_Prices`  
- `Daily_Returns`  
- `Beta_Alpha`  
- `CAPM_Returns`  

This Excel file can be **directly imported into Power BI** to build dashboards for:
- Risk comparison  
- Beta ranking  
- Expected return analytics  
- Performance benchmarking  

---

## 📊 Sample Outputs (Included in Repo)

This repository contains:
- Example visualizations (PNG exports)  
- `capm_output.xlsx` (generated using **AAPL, HBI, TSLA**)  

These serve as a reference for expected output structure.

---

## 🧠 What This Project Demonstrates

This project highlights skills in:

- Financial modeling using CAPM  
- Automated data pipelines  
- Regression-based risk estimation (beta/alpha)  
- Python-driven quantitative analysis  
- Interactive data visualization (Plotly)  
- Power BI dashboard integration  
- Multi-sheet Excel financial reporting  

Perfect for resumes, portfolios, and academic submissions.

---

## 🛠 Tech Stack

- **Python** (Colab / Jupyter)  
- **yfinance** (market data retrieval)  
- **pandas, numpy**  
- **scikit-learn** (linear regression)  
- **Plotly** (interactive graphs)  
- **OpenPyXL** (Excel export)  
- **Power BI** (dashboard visualization)

---

## 📐 CAPM Formula Used

\[
E[R] = R_f + \beta (R_m - R_f)
\]

Where:  
- **R_f** = annual risk-free rate  
- **R_m** = annualized market return  
- **β** = stock’s sensitivity to the market  

---



---

## 📁 Repository Structure

/project-root
│
├── README.md
├── capm_output.xlsx # Sample Excel output (AAPL vs HBI vs TSLA)
├── images/ # Sample Plotly exports
│ ├── price_history.png
│ ├── normalized_prices.png
│ ├── beta_scatter.png
│ └── secondary_axis_plot.png
│
└── capm_notebook.ipynb # Full CAPM analysis workflow
