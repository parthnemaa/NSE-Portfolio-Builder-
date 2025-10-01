# Portfolio Creation Using Equal Weight Strategy

**A Jupyter notebook to build and manage an equal weights portfolio with India’s top 50 stocks by market capitalization. Fetches real-time data, recommends optimal share distribution for any investment amount, and is suited for investors and finance students.**

---

**Project Purpose**
- **Helps construct diversified portfolios with India’s top listed companies by market capitalization.**
- **Ideal for beginner investors, finance students, and professionals prototyping equity allocation strategies.**

---

**Features**
- **Loads top 50 Indian stocks with ticker, company name, market cap, and latest price.**
- **Sorts stocks by market capitalization for portfolio inclusion.**
- **Calculates optimal shares to buy for a given investment using equal-weight allocation.**
- **Uses Python, pandas, numpy, and yfinance for data handling and retrieval.**

---

**How It Works**
- **Initial Setup:** Import libraries and load data (CSV or yfinance).
- **Data Processing:** Sort by market capitalization.
- **Allocation Calculation:** User enters investment; computes shares per stock for equal allocation.
- **Results Visualization:** View summary tables of share purchases and allocations.

---

**Requirements**
- Python 3.6+ (tested with Python 3.13.1)
- pandas
- numpy
- yfinance

---

**Getting Started**
- **Clone the repository and open Portfolio.ipynb in Jupyter.**
- **Run the cells to load and process stock data.**
- **Input total amount to allocate.**
- **View recommended share counts and allocation breakdown.**

---

**Example Usage**
- **Load Nifty constituent stocks.**
- **Enter investment (e.g., ₹1,00,000).**
- **Script recommends shares per stock for optimal diversification.**

---

**Who Should Use This Project**
- Finance students studying portfolio construction.
- Investors seeking guided allocation strategies.
- Researchers/professionals testing equal-weight methods on Indian market data.

---

**Extending the Project**
- Support weighting by market cap or volatility.
- Integrate live price APIs.
- Add portfolio rebalancing.

---

**Acknowledgements**
- yfinance for data
- pandas and numpy for wrangling
- JupyterLab for scripting

