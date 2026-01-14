# Impact of State-Level Socio-Economic Indicators on Startup Surge in India

This repository contains the complete data, code, and report for an econometric study examining how key state-level socio-economic factors influence startup activity across Indian States and Union Territories in 2021.

The study focuses on three major determinants:
- GDP per capita (economic development)
- Number of higher education institutions (human capital and institutional capacity)
- Public capital outlay (infrastructure and public investment)

The dependent variable is the number of DPIIT-recognized startups in each state and UT.

---

## Research Question

How do economic development, institutional capacity, and public investment affect the number of startups across Indian states?

---

## Data

The dataset consists of cross-sectional data for 32 Indian States and Union Territories for the year 2021.  
Sources include:
- Department for Promotion of Industry and Internal Trade (DPIIT)
- Reserve Bank of India (RBI)
- All India Survey on Higher Education (AISHE)

Variables:
- `startup_count` – Number of DPIIT-recognized startups
- `gdp_pc` – GDP per capita (₹, current prices)
- `uni_per_state` – Number of higher education institutions
- `capital_outlay` – State government capital outlay (₹ crore)

The dataset is stored in the `data/` folder.

---

## Methodology

The analysis uses multiple regression techniques with extensive diagnostic testing.  
Key steps include:

- Ordinary Least Squares (OLS) estimation
- Testing for heteroskedasticity (Breusch–Pagan and White tests)
- Testing for normality (Shapiro–Wilk and Anderson–Darling tests)
- Box–Cox transformation to correct non-normality
- Model selection using Mallows’ Cp, AIC, and BIC
- Multicollinearity checks using VIF, IVIF, correlation matrix, and eigenvalues
- Influence and outlier analysis using leverage, DFBETAS, Cook’s distance, and covariance ratio
- Model refinement after removing influential observations
- Type I and Type II ANOVA for robustness

---

## Repository Structure

