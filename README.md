# Modeling Pakistan’s Macroeconomic Dynamics  
## A Time Series Approach Using VAR, SVAR, and VECM

This repository presents an applied macroeconometric analysis of Pakistan’s economy using modern time series techniques. The study includes **univariate analysis** (time series plots, unit root tests, and ARIMA/ARMA models) as well as **multivariate analysis**, such as Vector Autoregression (VAR), Structural VAR (SVAR), and Vector Error Correction Models (VECM).

---

## 📈 Variables to be Used (Quarterly Data)

| Variable | Source | Notes |
|--------|--------|------|
| Real GDP | PBS / SBP | Convert to log, adjust for inflation |
| Government Spending | SBP / IMF IFS | Central government expenditure (real) |
| Tax Revenue | MoF / SBP | Net revenue or tax-to-GDP ratio |
| Inflation (CPI) | PBS | Quarterly average of CPI |
| Interest Rate | SBP (Policy Rate) | Used as-is |

---

## 🗃️ Data Sources
- State Bank of Pakistan (SBP)  
- Pakistan Bureau of Statistics (PBS)  
- IMF – International Financial Statistics (IFS) API  
- World Bank – World Development Indicators (WDI)  
- Ministry of Finance, Pakistan  

---

## 🧭 Project Tasks & Workflow

### 1️⃣ Data Collection & Cleaning
- Collect at least 11 years (44 quarters) of data  
- Convert variables into time series format  
- Log-transform and seasonally adjust where necessary  
- Plot and visually inspect all time series  

---

### 2️⃣ Univariate Time Series Analysis
- Plot and describe patterns for each variable  
- Conduct ADF and KPSS tests for stationarity  
- Apply log transformation and/or differencing  
- Fit ARIMA/ARMA models where relevant  

---

### 3️⃣ Vector Autoregression (VAR)
- Ensure all series are stationary  
- Select optimal lag length 
- Estimate the VAR model  
- Perform:
  - Granger causality tests  
  - Impulse Response Functions (IRFs)  
  - Forecast Error Variance Decomposition (FEVD)  

---

### 4️⃣ Structural VAR (SVAR)
- Impose short-run identification (AB-model)  
- Apply institutional restrictions (e.g., Blanchard–Perotti method)    
- Plot IRFs for:
  - Government spending → GDP and inflation  
  - Tax shocks → GDP  
  - Interest rate → inflation  

---

### 5️⃣ Cointegration and VECM
- Conduct Johansen cointegration tests    
- Interpret long-run cointegrating relationships  
- Explain short-run dynamics via error correction terms  

---

## 📃 Deliverables
- **Research Report** including:
  - Introduction  
  - Methodology  
  - Results and interpretation  
  - Policy implications for Pakistan  
- **Quarto Notebook**
- **Rendered HTML file** with complete code and graphical outputs
