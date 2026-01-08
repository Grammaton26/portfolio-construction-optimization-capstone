# Portfolio Construction and Optimization  
## Quantitative Approaches to Enhancing Investment Performance

This repository contains the code and supporting materials for the Capstone Project  
**“Portfolio Construction and Optimization: Quantitative Approaches to Enhancing Investment Performance.”**

The project evaluates traditional and data-driven portfolio construction methods using historical S&P 500 equity data, with a focus on performance comparison, downside-risk assessment, and sensitivity to market volatility.

---

## Project Objectives

The primary objective of this project is to evaluate whether modern quantitative techniques improve investment performance and risk management relative to traditional approaches. Specifically, the project addresses the following research questions:

- **RQ1:** How does a traditional Modern Portfolio Theory (MPT)–optimized portfolio compare to a machine-learning–based screening model in terms of risk-adjusted returns?
- **RQ2:** Do Monte Carlo simulations provide more reliable downside-risk insights than single-period optimization models?
- **RQ3:** How does market volatility affect the performance of MPT, machine-learning screening, and Monte Carlo–based risk analysis?

---

## Methods Overview

Three portfolio construction and evaluation approaches are implemented:

### 1. Modern Portfolio Theory (MPT)
- Mean–variance optimization
- Sharpe ratio maximization
- Long-only, fully invested constraints
- Out-of-sample performance evaluation

### 2. Machine-Learning–Based Screening
- Random Forest regression model
- Lagged momentum and volatility features
- Asset ranking and screening (not point prediction)
- Portfolio evaluation using consistent metrics

### 3. Monte Carlo Simulation
- 10,000 simulated one-year return paths
- Downside-risk estimation using:
  - Value-at-Risk (VaR)
  - Conditional Value-at-Risk (CVaR)
- Visualization of return distributions and tail risk

### Volatility Regime Analysis
- Market regimes defined using the CBOE Volatility Index (VIX)
- Performance evaluated separately under low-, medium-, and high-volatility conditions

---

## Technology Stack

- **Python** – Data preparation, modeling, simulation, and statistical analysis  
- **Key Libraries:** pandas, numpy, scipy, scikit-learn, matplotlib  
- **PostgreSQL** – Structured data storage and reproducibility support  
- **Tableau** – Visualization and presentation of analytical results  
- **GitHub** – Version control and documentation

---

## Dataset

- **Source:** *S&P 500 stock data: Historical stock data for all current S&P 500 companies* (Cam Nugent, Kaggle)  
- **Link:** https://www.kaggle.com/datasets/camnugent/sandp500  
- **Coverage:** Five years of daily trading data (2013–2018)  
- **Granularity:** One observation per stock per trading day  

---

## Reproducibility Instructions

To reproduce the analytical results:

1. Clone this repository
2. Install required Python libraries listed above
3. Download the dataset from Kaggle and place it in the appropriate directory
4. Run the Python script from start to finish

All figures, tables, and performance metrics presented in the final paper and presentation are generated directly from this script.

---

## PostgreSQL Integration (Optional)

The Python script includes an appendix section that exports selected datasets to CSV format for ingestion into a PostgreSQL database.

> These exports support structured storage and reproducibility but are **not required** to reproduce the analytical results.

---

## Project Deliverables

This repository supports the following Capstone deliverables:

- **Final Research Paper** – Detailed methodology, results, and hypothesis evaluation
- **Slide Presentation** – Executive-level summary of findings
- **Oral Presentation** – Recorded presentation of slides and results
- **Technical Documentation** – Code and reproducibility evidence (Module 8, Part 3)

---

## Disclaimer

This project is for academic and educational purposes only. The models and results presented here are intended as decision-support tools and do not constitute investment advice.
