Stock Data Analysis Project
This project performs exploratory, time-series, and performance analysis on daily stock market data using pandas. It is organized into 4 key tasks that automate data preparation, analysis, and reporting.

📂 Dataset Structure
stocks.csv – Daily stock prices (date, open, high, low, close, volume, Name)

fundamentals.csv – Company fundamentals (Ticker, Marketcap, Sector, etc.)

prices.csv – Current prices (Ticker, Currentprice)

data/ – Folder containing individual stock CSVs ({Name}.csv)

monthData/ – Folder for monthly resampled CSVs ({Name}.csv)

✅ Task Overview
🔹 Task 1: Data Exploration and Manipulation
Load stocks.csv and:

Compute average close price for each stock

Save to stock_data.csv

Calculate daily % change in close price

Save per-stock CSVs to data/{Name}.csv

🔹 Task 2: Time Series Analysis
Resample stock data to monthly frequency:

Average: open, high, low, close

Total: volume

Save results to monthData/{Name}.csv

Add 30-day rolling average of close to data/{Name}.csv

🔹 Task 3: Data Merging and Joining
Merge fundamentals.csv and prices.csv on Ticker

Compute Marketcap to Price ratio

Save merged results to stockInfo.csv

🔹 Task 4: Performance Analysis
For each stock in monthData/:

Calculate daily Profit/Loss (PnL) assuming buy on Day 1

Add Cumulative PnL and Drawdown

Save updated CSVs back to monthData/

