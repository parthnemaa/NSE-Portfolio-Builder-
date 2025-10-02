# NSE Portfolio Builder

An advanced Python project that builds an equal-weight portfolio using dynamic Indian stock data from NSE. Leveraging the `nsepython` package and Yahoo Finance (`yfinance`), it fetches real-time NSE stock symbols, fundamental data, and dynamically selects a top 50 universe by market capitalization.

## Features

- **Dynamic NSE Symbol Fetching:** Uses `nsepython` to get current NSE equity symbols without manual updates.
- **Live Stock Fundamentals:** Retrieves updated prices, market caps, P/E ratios, dividend yields from Yahoo Finance.
- **Market Cap Based Selection:** Selects top 50 stocks by market capitalization for portfolio inclusion.
- **Equal Weight Allocation:** Efficient calculation of shares to buy for any user-specified investment amount.
- **Enhanced Visualization:**
  - Stylish DataFrame tables with color-coded key metrics.  
- **User Friendly:** Validates user input and formats all financial numbers with Indian Rupee formatting and percentages.
- **Notebook Ready:** Designed for smooth execution and display in Jupyter Notebooks.

## Installation
pip install nsepython yfinance pandas matplotlib plotly

## Usage
1. Clone this repository:
git clone https://github.com/yourusername/nse-portfolio-builder.git
cd nse-portfolio-builder

2. Open the Jupyter Notebook `Portfolio.ipynb` or run the script.
3. Follow notebook cells to:
4. 
- Fetch NSE symbols dynamically.
- Fetch live fundamental data.
- Compute an equal-weight portfolio based on your investment.
- Visualize the portfolio using styled tables, interactive charts, and animations.

Example Python usage snippet:
After fetching and filtering top 50 stocks

investment = get_investment_amount() # Prompts user
portfolio_df = calculate_shares(portfolio_df, investment)
display_portfolio_animated(portfolio_df)


## Advantages

- **Automated Data Updating:** No manual maintenance of stock ticker lists required.
- **Real-time Market Data:** Ensures portfolio reflects current market conditions.
- **Visual Richness:** Tables and charts make portfolio allocations easy to analyze.
- **User Interaction:** Input validation and formatted results improve user experience.
- **Extensible:** Easy to add other portfolio strategies or visualization features.

## Known Issues

- Data fetching may slow for large symbol sets.  
- Requires stable internet for Yahoo Finance API connectivity.  
- Planned features and improvements are ongoing.

## Contributing
- Contributions and suggestions are welcome!
- Please open issues or pull requests for improvements, bug fixes, or new features.

## Made with ❤️ for easy and dynamic NSE portfolio management by **Parth Nema**








