

# Trading Strategies Analysis

[![License](https://img.shields.io/github/license/your-username/trading-strategies-analysis)](LICENSE)
[![Version](https://img.shields.io/badge/version-1.0.0-blue)](https://github.com/your-username/trading-strategies-analysis)
[![Python](https://img.shields.io/badge/Python-3.7%2B-brightgreen)](https://www.python.org/)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange)](https://jupyter.org/)

## Table of Contents

- [About the Project](#about-the-project)
- [Features](#features)
- [Directory Structure](#directory-structure)
- [Setup Instructions](#setup-instructions)
- [How to Run](#how-to-run)
- [Tools Description](#tools-description)
- [Notebook Analysis](#notebook-analysis)
- [Data Management and Security](#data-management-and-security) 
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

---

## About the Project

This project implements and evaluates various **trading strategies** to optimize performance in financial markets, specifically focusing on cryptocurrency prices. The project is centered on algorithmic trading and uses **Python**, **Jupyter notebooks**, and **Tableau** for strategy analysis, backtesting, and visualization.

---

## Features

- **Comprehensive Data ETL**: Automates the extraction and preprocessing of cryptocurrency data from multiple fiat currencies, ensuring well-structured data for analysis.
- **Algorithmic Trading Strategies**: Implement various algorithms to optimize returns and mitigate risks.
- **Backtesting**: Assess the historical performance of different strategies using real market data.
- **Tableau Visualizations**: Visualizations to easily compare the performance of strategies across timeframes and market conditions.

---

## Directory Structure

```bash
Trading_Strategies_Analysis-main/
├── README.md                    # Project documentation
├── Tableau WorkBook/             # Tableau workbook for visualizing strategy results
│   └── Dev Project.twb
├── etl/                          # ETL for cryptocurrency data
│   ├── AUD_btc_prices.csv
│   ├── CAD_btc_prices.csv
│   ├── ETL.ipynb                 # ETL process in Jupyter notebook
│   └── ...                       # Other fiat currency data
├── old strategies/               # Old trading strategies notebooks
│   └── Trading_Strategies_implementation.ipynb
├── preproccessing-data/          # Data preprocessing notebooks
│   └── preprocessed-dataset-for-strategies.ipynb
└── trading algorithms/           # Trading algorithms notebooks
    ├── Trading_Strategy.ipynb
    ├── trading_strategy_3.ipynb
    └── trading_stratergy_2.ipynb
```

---

## Setup Instructions

### Prerequisites

Ensure the following are installed on your system:

- **Python 3.7+**
- **Jupyter Notebook**
- **Tableau Desktop** (for viewing the visualizations)

---

## How to Run

### 1. Running ETL for Cryptocurrency Data

The `etl/ETL.ipynb` notebook processes cryptocurrency price data from various fiat currencies and loads it for analysis. Run this notebook to prepare data for analysis:

```bash
jupyter notebook etl/ETL.ipynb
```

### 2. Running Trading Strategies

Explore and evaluate different trading strategies by running the notebooks under `trading algorithms/`. For example, to run the main trading strategy:

```bash
jupyter notebook trading algorithms/Trading_Strategy.ipynb
```

The backtesting results will be displayed within the notebook, allowing you to see how different strategies perform under various market conditions.

---

## Tools Description

- **Python & Pandas**: Used for data manipulation and analysis of cryptocurrency price data.
- **Jupyter Notebooks**: Interactive notebooks used for backtesting trading strategies.
- **Tableau**: Used for visualizing the performance of each trading strategy.
- **Plotly & Matplotlib**: Libraries used for creating visualizations and graphs within the notebooks.

---

## Notebook Analysis

### 1. **ETL.ipynb (ETL Process)**

This notebook is responsible for extracting and preprocessing cryptocurrency data from different fiat currencies (such as AUD and CAD). The key steps involved include:

- **Data Extraction**: Imports raw cryptocurrency price data from CSV files.
- **Data Cleaning**: Handles missing values and ensures consistent time intervals for price data.
- **Data Transformation**: Converts data into a suitable format for use in trading algorithms (e.g., creating OHLC data frames).
- **Output**: Preprocessed data is saved for analysis by the trading strategy notebooks.

The ETL process is crucial for ensuring the quality and consistency of input data, which directly impacts the accuracy of the trading models.

### 2. **preprocessed-dataset-for-strategies.ipynb**

This notebook handles the preprocessing steps required for running trading strategies. It focuses on:

- **Feature Engineering**: Creating additional features (e.g., moving averages, volatility indicators) from the price data to improve the performance of trading strategies.
- **Data Splitting**: Splitting the data into training and testing sets to allow for backtesting of strategies.
- **Visualization**: Displays initial data visualizations to ensure that preprocessing steps have been applied correctly.

By engineering features and splitting the data, this notebook ensures the trading models have relevant inputs for training and evaluation.

### 3. **Trading_Strategy.ipynb**

This notebook implements a core trading strategy, utilizing technical indicators and backtesting the strategy using historical data. Key elements include:

- **Strategy Design**: Implements a moving average crossover strategy, where buy/sell signals are generated based on the crossover of short-term and long-term moving averages.
- **Backtesting**: Evaluates the historical performance of the strategy, calculating key metrics such as return on investment (ROI), drawdown, and win rate.
- **Visualizations**: Uses Plotly to visualize entry/exit points on price charts, providing a clear view of how the strategy performed over time.

This notebook provides a comprehensive implementation of a simple yet effective strategy, offering insights into the profitability of using moving averages in algorithmic trading.

### 4. **trading_strategy_2.ipynb & trading_strategy_3.ipynb**

These notebooks explore alternative trading strategies, each using different technical indicators and market conditions:

- **Strategy 2**: Focuses on momentum-based trading, where buy/sell signals are triggered based on the momentum of price movements.
- **Strategy 3**: Implements a Bollinger Bands strategy, where signals are generated when the price moves outside the upper or lower bands.

Both strategies include backtesting results, comparing performance metrics like profitability and risk against the baseline moving average crossover strategy.

---

## Data Management & Security

### **Data Management**:
This project ensures effective data handling through:
1. **ETL Process**: Automated extraction and transformation ensure clean and structured data.
2. **Data Preprocessing**: Creation of additional features improves the effectiveness of trading models.

### **Security Considerations**:
- **Privacy**: The dataset contains no personal information, ensuring user privacy is maintained.
- **Data Integrity**: Preprocessing steps ensure data quality and integrity, a crucial factor in algorithmic trading to avoid skewed results.

---


This video presentation offers a detailed overview of the project’s goals, outcomes, and technical components: https://github.com/Ankush2201/Trading_Strategie_Analysis/assets/79956433/af980674-1304-4cea-a7bd-0280ac5857c7


---
## Contributing

Contributions to this project are welcome. To contribute:
1. Fork the repository.
2. Create a feature branch (`git checkout -b feature-branch`).
3. Commit your changes (`git commit -m 'Added new feature'`).
4. Push to the branch (`git push origin feature-branch`).
5. Open a Pull Request.

---

