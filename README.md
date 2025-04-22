# MacroTrader

# MacroTrader: Macroeconomic Event Analysis for Equity Analysis

![Version](https://img.shields.io/badge/version-1.0.0-blue)
![Python](https://img.shields.io/badge/python-3.9%2B-blue)

<p align="center">
  <img src="docs/images/dashboard_preview.png" alt="MarketPulse Dashboard" width="750">
</p>

## 🔍 Overview

MacroTrader is a comprehensive analytics tool designed to help options traders capitalize on market overreactions to macroeconomic events. By monitoring FOMC meetings, Fed speeches, JOLTS reports, and other significant economic releases, MacroTrader identifies intraday volatility patterns and potential trading opportunities in SPY, TLT, and GLD.

My experience in financial market news revealed a persistent pattern: markets frequently overreact to macroeconomic news in the short term, creating temporary mispricing in equities and option premiums. MacroTrader was built to detect and provide actionable insights for short-term to mid-term trading strategies.

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
