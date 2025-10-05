# Crypto_Quant

> *"Turning market chaos into structured alpha — one model at a time."*

Welcome to **Crypto_Quant**, my personal journey of building and experimenting with algorithmic trading strategies in the cryptocurrency market.  
This project combines **quantitative analysis**, **backtesting**, and **machine learning** to explore systematic ways of trading Bitcoin, Ethereum, and other major tokens.

---

## Project Overview

This repository aims to develop and compare multiple quantitative strategies, starting from classical **technical indicator systems** and gradually evolving toward **AI-assisted trading agents**.

| Phase | Description                                     | Status        |
|------:|-------------------------------------------------|---------------|
| I     | RSI + Moving Average Strategy (Backtest)        | Completed  |
| II    | Feature Engineering (Volatility, Funding Rate)  | In progress |
| III   | ML-based Price Direction Classifier             | Planned    |
| IV    | Portfolio Optimization + Risk Management        | Upcoming   |

---

## Core Features

- **Data Pipeline** – Load & preprocess OHLCV (Binance / Bitget / Yahoo Finance).
- **Technical Strategies** – RSI, MACD, MA crossover, Bollinger Bands with tunable params.
- **Backtesting Engine** – Simulate trades; compute Returns, Sharpe, Max Drawdown, CAGR.
- **Visualization** – Signal overlays, equity curves, performance comparison.
- **(Optional) ML & AI** – Logistic/RandomForest/LSTM for short-term direction prediction.

---

## Tech Stack

| Category     | Tools |
|--------------|------|
| Language     | Python 3.10+ |
| Libraries    | Pandas, NumPy, Matplotlib, scikit-learn, TA-Lib, Backtesting.py |
| Data Source  | Binance API / Yahoo Finance |
| Visualization| Matplotlib / Plotly |
| Environment  | Jupyter Notebook / VS Code |

---

## Quick Start

~~~bash
# 1) Clone
git clone https://github.com/ceiceix/Crypto_Quant.git
cd Crypto_Quant

# 2) Install dependencies
pip install -r requirements.txt

# 3) Run example strategy
python main.py
~~~

Example output (Phase I):

~~~
Initial capital: $10,000
Final capital: $10,430
Sharpe Ratio: 1.21
Max Drawdown: -3.5%
~~~

---

## 📊 Results Preview

![Equity Curve Example](docs/preview_equity.png)

> RSI + MA crossover on BTC/USDT: **+4.3%** net gain over 7 days in a choppy market.  
> *(Replace the image with your own chart at `docs/preview_equity.png`.)*

---

## Folder Structure

~~~
Crypto_Quant/
├─ data/                 # Raw & processed data
├─ notebooks/            # Jupyter exploration
├─ src/                  # Core modules
│  ├─ data_loader.py
│  ├─ indicators.py
│  ├─ strategy.py
│  ├─ backtest.py
│  └─ metrics.py
├─ results/              # Backtest logs & charts
├─ docs/                 # README images & docs
├─ requirements.txt
└─ main.py               # Entry point
~~~

---

## Vision

Bridge **traditional quant logic** with **modern ML methods**, then evolve toward an **autonomous trading agent** that analyzes signals, predicts short-term moves, and adapts risk dynamically.

---

## To-Do

- [ ] Add data downloader (Binance REST & klines caching)  
- [ ] Implement position sizing & risk (ATR-based, Kelly-lite)  
- [ ] Add walk-forward analysis & hyper-param search  
- [ ] Introduce ML classifier baseline (LogReg / RF)  
- [ ] Compare against buy-and-hold & naive baselines

---

## Author

**Chang Xu (Cece)** – MEng, University of Toronto  
Focus: Quant trading • ML systems • Agent-based modeling


