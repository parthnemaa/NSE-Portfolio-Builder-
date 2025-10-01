# Portfolio Creation Using Equal Weight Strategy

A Jupyter notebook to build and manage an equal weights portfolio with India’s top 50 stocks by market capitalization. Fetches real-time data, recommends optimal share distribution for any investment amount, and is suited for investors and finance students.

Project Purpose
The main objective is to help users easily construct a diversified equity portfolio comprising India’s top listed companies based on market capitalization. This tool provides a step-by-step workflow from data loading to allocation, making it suitable for beginner investors, finance students, and professionals needing quick prototyping of allocation strategies.

Features
Loads a list of top 50 Indian stocks with ticker, company name, market capitalization, and latest trading price.
Automatically sorts stocks by market capitalization to identify leaders for portfolio inclusion.
Calculates the number of shares to purchase for each stock according to a user-defined investment amount using the equal-weight allocation method.
Uses Python, pandas, numpy, and yfinance for data import, manipulation, and retrieval; also supports visualization of allocations.

How It Works:
Initial Setup: Import required Python libraries and load stock data from CSV or via yfinance.
Data Processing: Sort stocks by market capitalization and extract the top selections for user analysis.
Allocation Calculation: User enters desired investment amount; the tool computes how many shares to buy for each stock to achieve equal allocation.
Results Visualization: Tables and outputs summarize the recommended share purchases and allocation breakdowns.

Requirements:

Python 3.6+ (tested with Python 3.13.1)
pandas
numpy
yfinance

Getting Started
Clone the repository and open Portfolio.ipynb in Jupyter.
Run cells to load the stock list and process the data.
Input the total amount to allocate when prompted.
View allocation outputs and summary tables for actionable investment guidance.

Example Usage
Load the list of Nifty constituent stocks.
Input that the planned investment is ₹1,00,000.
The script will output a breakdown showing suggested share count for each stock, optimizing capital usage and diversification.

Who Should Use This Project
Finance students learning about portfolio construction, allocation strategies, and Indian equity markets.
Individual investors and hobbyists wanting guided, data-driven portfolio decisions.
Researchers/professionals testing equal-weight approaches on local market data.

Extending the Project
Potential future enhancements:

Support for different weighting schemes (market cap, volatility).
Integration with APIs for live stock price updates.
Automated portfolio rebalancing features.

Acknowledgements
yfinance for market data.
pandas and numpy for data wrangling.
JupyterLab for interactive scripting.

This README is suitable for direct use on GitHub or similar platforms. Please update the repository name and adjust details if integrating additional features or data sources
