English · [Polski](https://github.com/narewskimichal/narewskimichal/blob/main/README_PL.md)

# Michał Narewski

**MSc Computer Science and Econometrics** · AGH University of Krakow · Data analysis · Financial analysis · Accounting

I analyse data with Python, SQL, Power BI and R, mostly on finance-related problems: housing prices, portfolio risk and trading strategies. 

Each project below has its own README with the question, the approach, charts and the main results, so you can get the idea in a couple of minutes.

## My Tools

- **Python:** pandas, NumPy, scikit-learn, XGBoost, TensorFlow/Keras, matplotlib, Jupyter
- **SQL:** PostgreSQL, data modelling, analytical queries
- **Power BI:** ETL in Power Query, DAX, data modelling, data visualization, dashboards
- **R:** time series and econometric models (GARCH, DCC-GARCH, BEKK), ggplot2
- **Other:** Copilot Studio, Git and GitHub, VS Code

## Business intelligence and data visualization

### [Housing affordability in Poland](https://github.com/narewskimichal/poland-housing-affordability)
**Python** (data cleaning) · **PostgreSQL** (SQL) · **Power BI** (ETL, DAX, dashboard) · **Copilot Studio** (AI agent)

- **Repository:** [poland-housing-affordability](https://github.com/narewskimichal/poland-housing-affordability)
- **Question:** how many square metres of a flat can an average salary buy in 15 Polish cities, and is it cheaper to buy or to rent?
- **Result:** one average monthly gross wage buys **1.19 m² in Katowice** but only **0.60 m² in Warsaw**, and the mortgage payment for a typical flat is **higher than rent in all 15 cities**.
- **Inside the repo:** [Python](https://github.com/narewskimichal/poland-housing-affordability/tree/main/python) · [SQL](https://github.com/narewskimichal/poland-housing-affordability/tree/main/sql) · [Power BI](https://github.com/narewskimichal/poland-housing-affordability/tree/main/powerbi) · [Copilot Studio](https://github.com/narewskimichal/poland-housing-affordability/tree/main/copilot)

## Financial econometrics

### [Minimum-variance portfolio on the Warsaw Stock Exchange](https://github.com/narewskimichal/mvp-portfolio-gpw)
**R** · portfolio optimisation · DCC-GARCH and BEKK models · backtesting · university project

- **Repository:** [mvp-portfolio-gpw](https://github.com/narewskimichal/mvp-portfolio-gpw)
- **Question:** do advanced covariance models reduce the risk of a portfolio of 5 WSE stocks (PZU, BNP Paribas, CD Projekt, Orange Polska, Orlen) compared with the sample covariance? Backtest 2019–2025 with 350 portfolio rebuilds.
- **Result:** **no**. Portfolio volatility was **21.4%** with the sample covariance and **21.2%** with DCC-GARCH, while BEKK came out the riskiest at **22.7%**.

### [GARCH Value-at-Risk backtest for Apple](https://github.com/narewskimichal/garch-var-backtest-aapl)
**R** · time series · GARCH volatility models · VaR backtesting (Kupiec, Christoffersen) · university project

- **Repository:** [garch-var-backtest-aapl](https://github.com/narewskimichal/garch-var-backtest-aapl)
- **Question:** which of 9 GARCH-type models gives reliable 95% VaR forecasts for Apple, with rolling windows of 100, 200 and 500 days?
- **Result:** **the window length mattered more than the model**. With 500 days **8 of 9 models** passed the Kupiec test, with 100 days **none** did. EGARCH fitted the full sample best but was the least reliable in forecasting.

## Machine learning (master's thesis)

### [Machine learning vs Buy & Hold on BTC](https://github.com/narewskimichal/btc-ml-vs-buy-and-hold)
**Python** · **machine learning** (XGBoost, logistic regression, LSTM) · walk-forward validation · backtesting 

- **Repository:** [btc-ml-vs-buy-and-hold](https://github.com/narewskimichal/btc-ml-vs-buy-and-hold)
- **Question:** do machine learning trading rules beat simply buying and holding BTC? Repeated on SPY, TLT and ETH.
- **Result:** on BTC the adaptive XGBoost strategy cut the maximum drawdown from **−77% to −30%** and raised the Sharpe ratio from **0.53 to 0.77**. The Sharpe gain is **not statistically significant** (p = 0.43) and does not hold on the other assets.
- **Inside the repo:** [Notebook with results](https://github.com/narewskimichal/btc-ml-vs-buy-and-hold/blob/main/analysis.ipynb) · [Thesis code](https://github.com/narewskimichal/btc-ml-vs-buy-and-hold/tree/main/thesis_code)

## Contact

If any of these projects caught your eye, feel free to reach out on [LinkedIn](https://www.linkedin.com/in/michal-narewski).
