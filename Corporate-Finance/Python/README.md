# Corporate Finance Coursework II: Python for Finance & Valuation Analysis

## Executive Summary
This repository contains Python-based financial models and analyses developed for Corporate Finance Coursework II. The coursework is structured to demonstrate the practical application of **Python for Finance**, progressing from foundational quantitative exercises to advanced empirical asset pricing (CAPM and Market Model event studies) and M&A valuation applied to **Pershing Square Holdings (PSH.L)**.

---

## Core Modules & Findings

### 1. General Quantitative Finance Exercises (Capital Budgeting)
* **Comparative Analysis:** Evaluates two mutually exclusive projects (Project A over 4 years vs. Project B over 3 years) under an 11% cost of capital.
* **NPV & Viability:** Both projects yield a **Positive Net Present Value** at 11% (Project A NPV = £15.27; Project B NPV = £113.05). However, under a 16% opportunity cost, Project A turns negative (NPV = -9.99), while Project B remains robust (NPV = 89.23).
* **Payback Period & Profitability Index (PI):** 
  * Project B achieves a faster payback (**2 years** vs. 3 years for Project A).
  * Project B exhibits a superior Profitability Index (**0.6** vs. **0.06** for Project A), confirming it as the optimal choice under capital rationing constraints.
* **Internal Rate of Return (IRR):** Project B delivers a significantly higher annualized return (**35.82%**) compared to Project A (**14.33%**).

### 2. Pershing Square Holdings: Asset Pricing & Event Study
* **CAPM & Beta Estimation:** Applied Python (statsmodels, yfinance) to regress monthly returns of PSH.L against the FTSE 100 benchmark (2014–2024), yielding a Beta of **0.8047** and a statistically significant Alpha of **0.0152**.
* **Market Efficiency & $R^2$:** The low $R^2$ (**0.205**) reflects structural differences between PSH's US-focused equity portfolio and its LSE listing, demonstrating how Python can diagnose index-asset mismatches.
* **Event Study (Nike Stake Increase - Nov 14, 2024):** 
  * Implemented an automated event study pipeline to extract pre-event estimation windows, compute expected returns via the Market Model, and calculate abnormal returns.
  * Results show negligible abnormal returns at $t=0$ ($-0.3\%$) and statistically insignificant $t$-statistics for Cumulative Abnormal Returns ($0.82\%$).
  * **Conclusion:** Consistent with the **semi-strong form of the Efficient Market Hypothesis (EMH)**, Python modeling proves that public disclosures are rapidly absorbed without exploitable post-event drift.

### 3. Pershing Square Holdings: M&A Valuation Model
* **Target Acquisition Valuation:** Programmed an automated M&A model to evaluate PSH acquiring **Scottish Mortgage Investment Trust Plc**.
* **Deal Metrics:** 
  * Standalone Target Equity Value: **£8,435.59M**
  * Offer Value (25% Premium): **£10,544.49M**
  * Deal Enterprise Value: **£11,095.49M**
  * PV of Synergies: **£2,778.46M**
  * **NPV to Acquirer:** **£669.56M** (indicates value creation).
* **EPS Impact & Financing:** Evaluated post-deal EPS dilution (falling from £0.40 to £0.20) and analyzed cash vs. stock financing mechanics through programmatic structures, demonstrating how Python handles complex corporate finance deal terms.

---

## Conclusions
1. **Bridging Theory and Code:** Working through these assignments allowed me to successfully translate core financial concepts—such as time value of money, risk-adjusted returns, and merger accretion/dilution—into clean, functional Python code.
2. **Mastering Financial Toolkits:** By utilizing libraries like pandas, numpy, statsmodels, and yfinance, I gained hands-on experience in managing end-to-end data pipelines, from fetching live market data to running robust econometric regressions.
3. **Applied Analytical Thinking:** Applying these quantitative techniques directly to Pershing Square Holdings helped me look past textbook formulas and understand how real-world market dynamics, structural currency mismatches, and information efficiency actually manifest in code.

---

## Practical Implications
1. **Confidence in Automated Modeling:** Building these scripts has given me the practical ability to move beyond static spreadsheets and build dynamic, reusable financial models that can quickly scale with new data.
2. **Empirical Rigor:** Implementing event studies and regression models hands-on taught me how to critically evaluate market anomalies, test hypotheses with statistical significance ($t$-stats), and avoid over-interpreting market noise.
3. **Readiness for Industry Applications:** The problem-solving frameworks and coding workflows developed in this project provide a solid foundation for tackling complex financial analysis, valuation tasks, and strategic decision-making in professional settings.
