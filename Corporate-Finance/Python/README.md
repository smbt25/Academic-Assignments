# Corporate Finance Coursework II: Python for Finance & Valuation Analysis

## Executive Summary
This repository contains Python-based financial models and analyses developed for Corporate Finance Coursework II. The project covers three core areas of financial decision-making: **Capital Budgeting & Investment Appraisal**, **Empirical Asset Pricing & Event Studies (CAPM & Market Model)**, and **Mergers & Acquisitions (M&A) Valuation**. The implementations demonstrate practical quantitative finance applications using Python (`pandas`, `numpy`, `yfinance`, `statsmodels`, and `matplotlib`).

---

## Key Modules & Findings

### 1. Capital Budgeting & Investment Appraisal (Project Evaluation)
* **Comparative Analysis:** Evaluates two mutually exclusive projects (Project A over 4 years vs. Project B over 3 years) under an 11% cost of capital.
* **NPV & Viability:** Both projects yield a **Positive Net Present Value** at 11% (Project A NPV = £15.27; Project B NPV = £113.05). However, under a 16% opportunity cost, Project A turns negative (NPV = -9.99), while Project B remains highly robust (NPV = 89.23).
* **Payback Period & Profitability Index (PI):** 
  * Project B achieves a faster payback (**2 years** vs. 3 years for Project A).
  * Project B exhibits a superior Profitability Index (**0.6** vs. **0.06** for Project A), confirming it as the superior choice under capital rationing constraints.
* **Internal Rate of Return (IRR):** Project B delivers a significantly higher annualized return (**35.82%**) compared to Project A (**14.33%**).

### 2. Asset Pricing & Event Study (Pershing Square Holdings vs. FTSE 100)
* **CAPM & Beta Estimation:** Regression analysis of monthly returns (2014–2024) yields a Beta of **0.8047** and a statistically significant Alpha of **0.0152**. 
* **Market Efficiency & $R^2$:** The low $R^2$ (**0.205**) highlights that PSH.L (investing primarily in large-cap US equities while listed in London) diverges from the FTSE 100 benchmark due to currency mismatches and active management strategies.
* **Event Study (Nike Stake Increase - Nov 14, 2024):** 
  * Analyzed abnormal returns around PSH's major stake announcement in Nike.
  * Both market-adjusted and Market Model regressions show negligible abnormal returns at $t=0$ ($-0.34\%$ / $-0.3\%$) and statistically insignificant $t$-statistics for Cumulative Abnormal Returns (CAR).
  * **Conclusion:** Consistent with the **semi-strong form of the Efficient Market Hypothesis (EMH)**, public information is priced in rapidly with no significant post-event drift.

### 3. Mergers & Acquisitions (M&A) Valuation
* **Target Acquisition:** Evaluates the acquisition of **Scottish Mortgage Investment Trust Plc** by Pershing Square Holdings.
* **Deal Metrics:** 
  * Standalone Target Equity Value: **£8,435.59M**
  * Offer Value (25% Premium): **£10,544.49M**
  * Deal Enterprise Value: **£11,095.49M**
  * PV of Synergies: **£2,778.46M**
  * **NPV to Acquirer:** **£669.56M** (indicates value creation).
* **EPS Impact:** Year-1 EPS experiences temporary dilution (falling from £0.40 to £0.20) due to financing costs and synergy realization lags.
* **Financing & Mispricing:** Examines cash vs. stock financing structures, demonstrating that cash-financed deals protect existing shareholders from sharing mispricing gains when target shares are undervalued.

---

## Conclusions
1. **Capital Budgeting Efficiency:** When evaluating competing investments, metrics like NPV, IRR, and Profitability Index collectively confirm that lower initial outlays coupled with front-loaded cash inflows (Project B) maximize shareholder wealth and capital efficiency.
2. **Empirical Market Behavior:** Stock return regressions and event studies validate market efficiency frameworks, showing that active management generates alpha while public announcements are swiftly absorbed without exploitable post-event drift.
3. **Strategic M&A Justification:** While M&A transactions can create substantial economic value (positive NPV through synergies), short-term accounting metrics like EPS dilution must be managed alongside long-term intrinsic value strategies.

---

## Practical Implications
* **Capital Allocation:** Financial managers should prioritize Profitability Index and capital-rationing models when resources are restricted, ensuring optimal deployment per unit of investment.
* **Risk & Benchmark Selection:** Analysts must account for structural mismatches (such as cross-border asset exposure vs. local index listing) when computing Betas and cost of equity.
* **M&actic Structuring:** Acquirers should carefully evaluate cash versus stock financing decisions based on market misvaluation signals and the timeline of synergy realization to protect existing shareholder value.
