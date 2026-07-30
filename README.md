# Boopesh Mohanraj

**Experience:**

· Junior Risk Officer & Junior Equity Research Analyst , 360 Huntington Fund (student-run, ~$2M AUM), Boston, MA

· Quantitative Research Analyst Intern, Global Delta Capital, Boston, MA

· Business Manager - Retail Fuel Distribution, Bharat Petroleum Corporation Limited (Authorized Bharat Petroleum Retail Dealership outlet), India

**Open to full-time finance roles** across investment research, portfolio and asset management, and risk.

---

## Quantitative Finance

| Project | Built & found | Stack |
| --- | --- | --- |
| **[Dynamic-Var-stress-testing-engine](https://github.com/BoopeshMohanraj/Dynamic-Var-stress-testing-engine)** · *[live dashboard](https://dynamic-var-stress-testing-engine-rk3qwtdff5nyyftrtqsfla.streamlit.app/)* | Historical, Parametric and Monte Carlo VaR, Expected Shortfall at 97.5% (FRTB), Filtered Historical Simulation with EWMA / GARCH(1,1) / GJR-GARCH, Kupiec and Christoffersen backtesting, Mean-CVaR optimization, macro sensitivity regression, SQL reporting.<br>*Static VaR failed Kupiec on 2022 while the filtered models tracked the regime, but GJR showed breach clustering, so no model won outright. Mean-CVaR cut in-sample 95% CVaR from 19.0% to 3.0%, then underperformed equal-weight through the 2022 duration shock.* | Python, arch, cvxpy, statsmodels, SQLite, Streamlit |
| **[Derivatives-Pricing-Heston-Calibration-Structured-Products](https://github.com/BoopeshMohanraj/Derivatives-Pricing-Heston-Calibration-Structured-Products)** | Black-Scholes and CRR binomial from first principles, all five Greeks analytically, delta-hedging simulation with Gamma decomposition, live SPY implied-vol surface, Heston calibration, NN price approximators, principal-protected note.<br>*Reproduces the equity skew that flat-vol BSM cannot price (live SPY: 19% ATM vs 39% at 10% OTM puts). Heston was calibrated to a synthetic smile rather than the market surface, stated as a limitation.* | Python, SciPy, PyTorch, yfinance, FRED |
| **[Fixed-Income-yield-curve-analytics](https://github.com/BoopeshMohanraj/Fixed-Income-yield-curve-analytics)** | Nelson-Siegel fitting, Vasicek three-factor term structure with a Kalman filter written in pure NumPy, GARCH/EGARCH bond vol with time-varying DV01 VaR, LSTM and VAR comparison, weekly PDF tear sheet.<br>*Kalman level factor turned up roughly a year before the first 2022 hike; GARCH caught a 2.5x vol rise Dec 2021 to Jun 2022. Vasicek/Kalman best at 1-month, VAR best at 3-month, and the LSTM did not converge on ~180 monthly observations, reported rather than dropped.* | Python, statsmodels, arch, PyTorch, FRED |
| **[Credit-risk-model-validation](https://github.com/BoopeshMohanraj/Credit-risk-model-validation)** | Merton structural model solved from public filings, Altman Z-Score and Beneish M-Score screening, PD/LGD/EAD/CVA with economic capital, Kaplan-Meier survival curves, champion-challenger validation on Gini / AUC / KS with PSI drift monitoring under SR 11-7.<br>*Merton output is risk-neutral PD, not a physical default probability, and is labeled that way throughout.* | Python, SciPy, scikit-learn, SEC EDGAR |
| **[Equity-signal-validation-Regime-detection](https://github.com/BoopeshMohanraj/Equity-signal-validation-Regime-detection)** | Factor replication on a 2015-2024 large/mid-cap universe: Engle-Granger cointegration pairs, 12-1 momentum with IC decay and Fama-MacBeth testing, Fourier seasonality, HMM regime detection, Almgren-Chriss impact, expanding-window walk-forward.<br>*No exploitable unconditional edge: Fama-MacBeth t-stat insignificant, no backtested pair significant at 5%. Regime-conditional selection improved in-sample results but did not survive walk-forward validation. That null result is the finding.* | Python, statsmodels, hmmlearn, Tiingo |

---

## Applied ML & Data Science

| Project | Description | Stack |
| --- | --- | --- |
| **[FRCOY-Stock-Forecasting-with-ATS-volume-VIX](https://github.com/BoopeshMohanraj/FRCOY-Stock-Forecasting-with-ATS-volume-VIX)** | Directional forecasting using FINRA ATS (dark pool) volume and VIX as alternative data | XGBoost, TensorFlow, Optuna |
| **[Bankruptcy-Prediction-Using-Python](https://github.com/BoopeshMohanraj/Bankruptcy-Prediction-Using-Python)** | Bankruptcy classification on imbalanced data (3.2% positive class), evaluated on recall and ROC-AUC. *Group* | scikit-learn, XGBoost |
| **[Sentiment-analysis-on-NYSE-JPM-using-python](https://github.com/BoopeshMohanraj/Sentiment-analysis-on-NYSE-JPM-using-python)** | Exploratory study of headline sentiment (VADER) against JPMorgan price action | NLTK, yfinance |
| **[Consumer-Segmentation-Running-Footwear](https://github.com/BoopeshMohanraj/End-to-End-Data-Quality-Driven-Consumer-Segmentation-for-the-Running-Footwear-Market)** | Four clustering algorithms compared by silhouette score; GMM chosen over KMeans for binary features. *Group* | scikit-learn, PCA |
| **[MedIScan](https://github.com/BoopeshMohanraj/MedIScan)** | Clinical-document pre-screening API with dual-model inference and OpenFDA lookup. *Group hackathon* | FastAPI, PyTorch, React |

Also here: statistical testing on US health insurance coverage, geospatial site selection, and a cross-chain transaction-monitoring pipeline. The last two are methods demonstrations on synthetic data, documented as such.

---

## Toolkit

| | |
| --- | --- |
| **Languages & data** | Python, SQL, Excel · FRED, Tiingo, yfinance, SEC EDGAR, FINRA |
| **Risk** | VaR / CVaR / Expected Shortfall, EWMA · GARCH · GJR-GARCH, Filtered Historical Simulation, Kupiec and Christoffersen testing, stress testing, Basel III and FRTB |
| **Derivatives & rates** | Black-Scholes and binomial pricing, five Greeks, delta hedging, vol surfaces, Heston calibration, Nelson-Siegel, Vasicek, Kalman filtering, DV01 |
| **Credit & portfolio** | Merton, Altman Z-Score, PD/LGD/EAD/CVA, Gini / AUC / KS, PSI, SR 11-7, Mean-variance and Mean-CVaR optimization, Fama-French attribution |
| **ML** | XGBoost, LSTM, HMM, PCA, model validation |

---
