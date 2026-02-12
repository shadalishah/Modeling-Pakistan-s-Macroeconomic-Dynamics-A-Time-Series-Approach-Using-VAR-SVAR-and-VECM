# Modeling-Pakistan’s-Macroeconomic-Dynamics-A-Time-Series-Approach-Using-VAR-SVAR-and-VECM
This repository presents an applied macroeconometric analysis of Pakistan’s economy using modern time series techniques, including univariate analysis (time series plots, unit root tests, and ARIMA/ARMA models) and multivariate analysis such as Vector Autoregression (VAR), Structural VAR (SVAR), and Vector Error Correction Models (VECM).
<b>
📈 Variables to be Used (Quarterly Data)
Variable	Source	Notes
Real GDP	PBS / SBP	Convert to log, adjust for inflation
Govt Spending	SBP / IMF IFS	Central Govt Expenditure (Real)
Tax Revenue	MoF / SBP	Use Net Revenue or Tax-to-GDP
Inflation (CPI)	PBS	Quarterly average of CPI
Interest Rate	SBP (Policy Rate)	Use as-is
<b>
3 🗃️ Data Sources
State Bank of Pakistan
Pakistan Bureau of Statistics
[IMF IFS Data API]
World Bank WDI
Ministry of Finance
<b>
4 🧭 Project Tasks & Workflow
4.1 1. Data Collection & Cleaning
Collect at least 10 years (40 quarters) of data
Log-transform and seasonally adjust if necessary
Plot and visually inspect time series
<b>
4.2 2. Univariate Time Series Analysis
Plot and describe patterns for each variable
Run ADF and KPSS tests for stationarity
Log and/or difference the data
Fit ARIMA models where relevant
<b>
4.3 3. Vector Autoregression (VAR)
Ensure all series are stationary
Use VARselect() for lag length selection
Estimate VAR model
Perform:
Granger causality tests
Impulse Response Functions (IRFs)
Forecast Error Variance Decomposition (FEVD)
<b>
4.4 4. Structural VAR (SVAR)
Impose short-run (AB-model) identification
Use institutional knowledge (e.g., BP method)
Estimate SVAR using svars or vars package
Plot IRFs for:
Govt spending → GDP, inflation
Tax → GDP
Interest rate → Inflation
<b>
4.5 5. Cointegration and VECM
Johansen cointegration test
Estimate VECM using tsDyn or urca
Interpret long-run cointegrating vectors
Explain short-run adjustments via error correction terms
<b>
5 📃 Deliverables
Report with:

Introduction
Methodology
Results and interpretation
Policy implications for Pakistan
Quarto Notebook and rendered html file with full code and graphs
