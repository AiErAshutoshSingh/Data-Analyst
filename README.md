# Stock Analysis with Pandas (Excel Data)

This project performs data analysis on stock price and company fundamentals using **Pandas** and **Excel files**.

It includes:
- Data manipulation
- Time series analysis
- Performance metrics
- Merging fundamentals with price data

---

##  Files Required

Upload these Excel files to your project or Google Colab:

| File Name         | Description                                 |
|------------------|---------------------------------------------|
| `stocks.xlsx`     | Daily stock prices (date, open, close, etc.) |
| `fundamentals.xlsx` | Company data like Ticker, MarketCap, Sector |
| `prices.xlsx`     | Price data for each Ticker                  |

---

## Tasks Completed

### 🔹 Task 1: Data Exploration and Manipulation
- Read stock data from `stocks.xlsx`
- Calculate average closing price per ticker
- Save per-ticker CSVs in `data/{Name}.csv`

### 🔹 Task 2: Time Series Analysis
- Resample stock data to monthly averages
- Save monthly data to `monthData/{Name}.csv`
- Add 30-day rolling average of close price

### 🔹 Task 3: Merging and Joining
- Merge `fundamentals.xlsx` and `prices.xlsx` on `Ticker`
- Calculate MarketCap / Price ratio
- Save result to `stockInfo.csv`

### 🔹 Task 4: Performance Analysis
- For each ticker:
  - Calculate daily PnL
  - Cumulative PnL
  - Drawdown
- Save updated files to `data/{Name}.csv`

---

## 🛠️ How to Run

###  In Google Colab

1. Upload all `.xlsx` files
2. Run each code block from `task1–4`
3. Outputs will be saved in:
   - `data/` — per stock data with PnL
   - `monthData/` — resampled monthly data
   - `stock_data.csv`, `stockInfo.csv`


pip install pandas openpyxl xlrd
