# 📊 NSE Portfolio Builder & Optimizer

> **A data-driven portfolio management system leveraging Modern Portfolio Theory to construct and optimize equity portfolios using NSE-listed stocks.**

[![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)](https://www.python.org/downloads/)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange.svg)](https://jupyter.org/)

---

## 🎯 Project Overview

This project builds an intelligent portfolio optimization system that helps retail investors and wealth managers construct optimal portfolios from India's top NSE-listed stocks. By applying **Modern Portfolio Theory** and **Monte Carlo simulation**, it identifies portfolios that maximize risk-adjusted returns.

### **Key Features**

✅ **Real-Time Data Integration** - Fetches live stock prices, fundamentals, and market data from NSE  
✅ **Portfolio Optimization** - Monte Carlo simulation with 10,000 random portfolios  
✅ **Efficient Frontier Visualization** - Interactive risk-return tradeoff analysis  
✅ **Risk Analytics** - Sharpe ratio, volatility, correlation, and diversification metrics  
✅ **Interactive Portfolio Builder** - User inputs investment amount and risk tolerance to get personalized allocations  
✅ **Sector Diversification** - Automated sector allocation analysis  
✅ **CSV Export** - Downloadable portfolio allocation ready for broker execution

---

## 💼 Business Problem

**Challenge:**  
Retail investors struggle to construct diversified, risk-optimized portfolios from thousands of NSE stocks without quantitative tools or financial expertise. Traditional investing often leads to:
- Over-concentration risk
- Suboptimal risk-adjusted returns
- Lack of systematic diversification

**Solution:**  
An automated portfolio optimization system that:
- Selects top stocks by market capitalization
- Calculates optimal weights using Modern Portfolio Theory
- Provides personalized allocations based on risk tolerance
- Generates actionable investment recommendations

---

## 🛠️ Tech Stack

| Category | Technologies |
|----------|-------------|
| **Language** | Python 3.8+ |
| **Data Sources** | `yfinance`, `nsepython` (NSE API) |
| **Analysis** | `pandas`, `numpy`, `scipy` |
| **Optimization** | Monte Carlo Simulation, Markowitz Mean-Variance |
| **Visualization** | `plotly`, `matplotlib`, `seaborn` |
| **Environment** | Jupyter Notebook |

---

## 📈 Methodology

### **1. Data Collection**
- Fetch 2,000+ NSE equity symbols via `nsepython`
- Retrieve fundamentals: price, market cap, P/E ratio, sector
- Select **top 50 stocks** by market capitalization
- Download **3 years of historical daily prices**

### **2. Portfolio Optimization**
- Calculate daily returns and covariance matrix
- Generate **10,000 random portfolios** via Monte Carlo simulation
- Compute for each portfolio:
  - Expected annual return
  - Annual volatility (risk)
  - Sharpe ratio (risk-adjusted return)
- Identify optimal portfolios:
  - **Maximum Sharpe Ratio** (best risk-adjusted returns)
  - **Minimum Volatility** (lowest risk)

### **3. Risk Analysis**
- **Correlation heatmap** - Stock relationship analysis
- **Sector allocation** - Diversification across industries
- **Sharpe ratio** - Return per unit of risk (target > 1.0)
- **Efficient frontier** - Visualization of optimal portfolios

### **4. Interactive Portfolio Builder**
User inputs:
- Investment amount (₹)
- Risk tolerance (Low/Medium/High)

System outputs:
- Personalized portfolio allocation
- Exact number of shares to buy for each stock
- Sector diversification breakdown
- Future portfolio value projections (1, 3, 5, 10 years)
- Actionable recommendations
- CSV export for broker execution

---

## 🚀 Getting Started

### **Prerequisites**

```bash
Python 3.8 or higher
Jupyter Notebook or JupyterLab
```

### **Installation**

1. **Clone the repository**
```bash
git clone https://github.com/parthnemaa/nse-portfolio-builder.git
cd nse-portfolio-builder
```

2. **Install dependencies**
```bash
pip install -r requirements.txt
```

3. **Launch Jupyter Notebook**
```bash
jupyter notebook NSE-2.ipynb
```

### **Dependencies**

```
yfinance>=0.2.0
nsepython>=2.0.0
pandas>=1.5.0
numpy>=1.23.0
scipy>=1.9.0
matplotlib>=3.6.0
plotly>=5.11.0
seaborn>=0.12.0
```

---

## 📊 Sample Results

### **Portfolio Performance Metrics**

| Portfolio Type | Annual Return | Volatility | Sharpe Ratio |
|---------------|---------------|------------|--------------|
| Equal Weight (Baseline) | 15.2% | 22.1% | 0.68 |
| Maximum Sharpe | 18.7% | 20.3% | 0.92 |
| Minimum Volatility | 12.4% | 16.8% | 0.74 |

*Sample data - actual results vary based on market conditions*

### **Top Holdings Example**

| Company | Sector | Weight | Shares | Investment |
|---------|--------|--------|--------|------------|
| Reliance Industries | Energy | 8.2% | 15 | ₹20,500 |
| TCS | IT Services | 7.5% | 6 | ₹18,750 |
| HDFC Bank | Banking | 6.8% | 12 | ₹17,000 |
| Infosys | IT Services | 6.3% | 10 | ₹15,750 |

### **Sector Allocation**

```
Financial Services    28.5% ████████████████████████████
IT Services          22.3% ██████████████████████
Energy               15.2% ███████████████
Consumer Goods       12.8% ████████████
Healthcare            8.7% ████████
Others               12.5% ████████████
```

---

## 🎯 Use Cases

### **For Retail Investors**
- Construct scientifically optimized portfolios
- Get exact share allocations for any investment amount
- Understand risk-return tradeoffs
- Download ready-to-execute trading lists

### **For Wealth Managers**
- Generate client-specific portfolio recommendations
- Match portfolios to client risk tolerance
- Automate portfolio rebalancing calculations
- Provide data-backed investment rationale

### **For Finance Students**
- Learn Modern Portfolio Theory implementation
- Understand Monte Carlo simulation
- Practice with real market data
- Build portfolio analysis skills

---

## 📂 Project Structure

```
nse-portfolio-builder/
│
├── NSE-2.ipynb                 # Main analysis notebook
├── README.md                   # Project documentation
├── requirements.txt            # Python dependencies
├── portfolio_allocation_*.csv  # Exported allocations (generated)
└── LICENSE                     # MIT License
```

---

## 🔮 Future Enhancements

- [ ] **Backtesting Module** - Compare portfolio performance vs NIFTY 50 benchmark
- [ ] **Streamlit Dashboard** - Interactive web app for real-time portfolio building
- [ ] **Automated Rebalancing** - Trigger alerts when positions drift >5%
- [ ] **Tax-Loss Harvesting** - Identify optimization opportunities
- [ ] **Machine Learning** - Predict optimal sector allocations
- [ ] **Multi-Period Optimization** - Dynamic rebalancing strategies
- [ ] **API Integration** - Real-time portfolio tracking
- [ ] **Mobile App** - iOS/Android portfolio monitoring

---

## 💡 Key Insights

### **What This Project Demonstrates**

**Finance Domain Knowledge:**
- Modern Portfolio Theory (Markowitz optimization)
- Risk metrics: Sharpe ratio, volatility, correlation
- Portfolio construction and diversification principles
- Efficient frontier analysis

**Technical Skills:**
- Python programming (pandas, numpy, scipy)
- API integration and data fetching
- Statistical analysis and Monte Carlo simulation
- Data visualization (plotly, matplotlib, seaborn)
- Interactive Jupyter notebook development

**Business Acumen:**
- Translating financial theory into practical tools
- User-centric design (investment amount input)
- Actionable recommendations and insights
- Production-ready output (CSV export)

---

## 📫 Contact

**Parth Nema**  
Finance Graduate | Data Analytics Enthusiast  

- **GitHub:** [@parthnemaa](https://github.com/parthnemaa)
- **LinkedIn:** [Connect with me](https://linkedin.com/in/parthnemaa)
- **Email:** your.email@example.com

---

## 🙏 Acknowledgments

- **Data Sources:** Yahoo Finance API, NSE Python Library
- **Inspiration:** Modern Portfolio Theory by Harry Markowitz
- **Community:** Python finance and data science communities

---

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## ⚠️ Disclaimer

**IMPORTANT NOTICE:**

This project is for **educational and research purposes only**. It is NOT investment advice.

- Past performance does not guarantee future results
- All investments carry risk, including potential loss of principal
- Portfolio optimization based on historical data may not predict future performance
- This analysis does not consider individual financial situations, risk tolerance, or investment objectives
- Transaction costs, taxes, and market impact are not included in calculations

**Before making any investment decisions:**
- Consult with a qualified financial advisor
- Conduct your own due diligence
- Understand your risk tolerance and investment horizon
- Consider all costs and tax implications

The author assumes no liability for any financial losses resulting from the use of this analysis.

---

## ⭐ Star This Repository

If you found this project useful, please consider giving it a star! It helps others discover this work and motivates further development.

---

**Built with ❤️ for the finance and data science community**
