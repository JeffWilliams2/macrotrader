# MacroTrader

# MacroTrader: Macroeconomic Event Analysis for Equity Analysis

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-232F3E?style=for-the-badge&logo=amazon-aws&logoColor=white)

## 🔍 Overview

MacroTrader is a comprehensive analytics tool designed to help traders capitalize on market overreactions to macroeconomic events. By monitoring FOMC meetings, Fed speeches, JOLTS reports, and other significant economic releases, MacroTrader identifies intraday volatility patterns and potential trading opportunities in SPY, TLT, and GLD.

<p align="center">
  <img src="/images/macro.png" alt="MarketPulse Dashboard" width="750">
</p>

# Trading Thesis: Market Overreactions to Macroeconomic Events

## Core Thesis

Markets systematically overreact to high-impact macroeconomic announcements in the short term, creating temporary mispricing in options premiums that can be exploited through strategic positioning. This inefficiency occurs because:

1. **Initial Volatility Spike**: Markets process macroeconomic data releases (FOMC minutes, JOLTS reports, CPI data) with immediate, often exaggerated price movements
2. **Volatility Mean Reversion**: This heightened volatility typically reverts toward the mean within 24-48 hours
3. **Options Mispricing Window**: During this reversion period, options premiums often remain elevated longer than warranted by the actual sustained market impact

## Observations

Through analysis of market behavior surrounding key economic events over the past five years (2020-2025), I've observed several consistent patterns:

- SPY typically exhibits a 0.7-1.2% intraday move following FOMC announcements, but 60-70% of this movement is typically retraced within the next trading session
- TLT (Treasury bond ETF) shows even more pronounced overreactions to interest rate commentary, with initial moves frequently being partially reversed
- GLD (gold ETF) demonstrates heightened sensitivity to inflation data, creating opportunities when correlated with bond movements

## Risk Management Framework

While the core thesis has demonstrated consistent validity, effective implementation requires rigorous risk management:

- Position sizing limited to 1-3% of portfolio per trade
- Defined stop-loss mechanisms based on volatility thresholds rather than just price levels
- Diversification across uncorrelated economic event types

## ✨ Key Features

- **Economic Calendar Integration**: Tracking of FOMC meetings, Fed speeches, JOLTS reports, CPI releases, Earning Reports and other market-moving events
- **Real-time Market Data Analysis**: Continuous monitoring of SPY, TLT, and GLD price action and volatility metrics surrounding key events
- **Options Premium Analyzer**: Identifies unusual options pricing and implied volatility expansions/contractions
- **Historical Pattern Recognition**: Compares current market reactions to previous similar events
- **Interactive Visualization Dashboard**: Clean, actionable views of market correlations and event impacts
- **Alert System**: Customizable notifications for potential trading opportunities

## 🚀 Getting Started

### Prerequisites

- Python 3.9+
- Pandas, NumPy
- MongoDB
- AWS account (for Notifications/Lambda and S3 functionality)
- Financial data API access (Yahoo Finance API, FRED, etc.)
- Knowledge of underlying financial markets. (Most important)

## 📊 Architecture

MacroTrader employs a modular data pipeline architecture:

1. **Data Collection Layer**: AWS Lambda functions that collect economic data from various sources and store in S3
2. **Processing Layer**: Python-based ETL pipeline with MongoDB for structured storage
3. **Analysis Engine**: Statistical models for volatility analysis and pattern recognition
4. **Visualization Layer**: Interactive dashboard built with Plotly and Streamlit

## 📈 Trading Strategy Context

MacroTrader is designed specifically for intraday options trading strategies focused on volatility reversion. The core thesis:

1. Macroeconomic announcements create immediate, often exaggerated market reactions
2. Options premiums frequently overprice the sustained impact of these events
3. By identifying historical patterns and current deviations, traders can capitalize on the reversion to normal volatility levels

The tool is particularly effective for:
- Selling short-term options during volatility spikes
- Identifying asymmetric reactions between SPY, TLT, and GLD
- Executing calendar spreads around scheduled economic events

## 🔄 Ongoing Development

Current development priorities:
- [ ] Integration with alpaca/thinkorswim APIs for automated execution
- [ ] Machine learning deploy to SageMaker
- [ ] Expanded asset coverage (sector ETFs, individual stocks)
- [ ] Real-time Fed speech sentiment analysis using NLP
- [ ] VIX futures and term structure analysis

## 🛠️ Tech Stack

- **Data Engineering**: Python, Pandas, Apache Airflow
- **Storage**: MongoDB, AWS S3
- **Processing**: AWS Lambda, PyTorch (for ML components)
- **Visualization**: Plotly, Streamlit
- **Deployment**: Docker, AWS

## 🙋‍♂️ About Me

Finance professional with a passion for quantitative analysis.

**Connect with me on [LinkedIn](https://www.linkedin.com/in/jefferywilliams4)**
