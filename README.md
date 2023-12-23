# Unsupervised Learning Trading Strategy

## Introduction

This project aims to develop an unsupervised learning-based trading strategy utilizing various financial indicators and machine learning techniques. The strategy involves data collection from Yahoo Finance, feature engineering, data processing, factor models, clustering, portfolio optimization, and backtesting.

## Project Structure

The project is organized as follows:

- **data:** Contains financial data collected from Yahoo Finance.
- **notebooks:** Jupyter notebooks for exploratory data analysis, modeling, and backtesting.
- **src:** Source code for data processing, feature engineering, and portfolio optimization.
- **results:** Output files, including portfolio returns and visualizations.

## Major Files and Directories

- **data_collector.py:** Python script for collecting financial data from Yahoo Finance.
- **feature_engineering.py:** Module for calculating key financial indicators.
- **portfolio_optimizer.py:** Module for portfolio optimization using the Efficient Frontier.
- **clustering.py:** Module for K-Means clustering of assets.
- **backtesting.py:** Module for backtesting the trading strategy.

## Data Collection

The project collects financial data using the Yahoo Finance API and utilizes the S&P 500 list for stock symbols.

## Feature Engineering

Key financial indicators are calculated, including Garman-Klass Volatility, RSI, Bollinger Bands, ATR, MACD, and Dollar Volume.

## Data Processing

Data is aggregated to the monthly level, and the top 150 most liquid stocks are filtered for each month. A 5-year rolling average of dollar volume is also calculated.

## Factor Models and Betas

Fama-French factors are used, and rolling factor betas are calculated using statsmodels.

## Clustering and K-Means

Assets are grouped using K-Means clustering, and the clusters are visualized.

## Portfolio Optimization

The portfolio optimization function is defined, and portfolio weights are optimized using the Efficient Frontier max sharpe ratio.

## Portfolio Backtesting

A portfolio backtesting strategy is implemented, and portfolio returns are compared to SP500 returns.

## Visualization

Graphical representation of portfolio returns over time is provided, along with a comparison with SP500 returns.

## Dependencies

- pandas
- numpy
- yfinance
- matplotlib
- statsmodels
- pandas_ta
- pypfopt
- scikit-learn

## Usage

1. Install dependencies: `pip install -r requirements.txt`
2. Execute notebooks in the `notebooks` directory for detailed analysis.
3. Run individual scripts in the `src` directory for specific tasks.

## Contributing

Feel free to contribute to the project by opening issues or submitting pull requests. See [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines.

## License

This project is licensed under the [MIT License](LICENSE).

## Acknowledgments

- Credits to the Yahoo Finance API for providing financial data.
- Thanks to the contributors and maintainers of the project dependencies.

## Future Work

- Implement additional trading strategies.
- Improve backtesting techniques.
- Explore alternative clustering algorithms.
