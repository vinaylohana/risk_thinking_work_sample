
# Problem 1: Raw Data Processing

## process_data.py
This Python script processes historical stock and ETF data from CSV files (sourced from https://www.kaggle.com/datasets/jacksoncrow/stock-market-dataset), and combines it into a single structured dataset in the Parquet format. The resulting dataset contains the following columns:

- Symbol: string
- Security Name: string
- Date: string (YYYY-MM-DD)
- Open: float
- High: float
- Low: float
- Close: float
- Adj Close: float
- Volume: int

# Problem 2: Feature Engineering

## transform_data.py
This code calculates the 30-day moving average of trading volume and the rolling median of adjusted close for a Parquet file containing stock and ETF data. The resulting dataset is saved as a new Parquet file, and contains the following columns:

- Symbol: string
- Security Name: string
- Date: string (YYYY-MM-DD)
- Open: float
- High: float
- Low: float
- Close: float
- Adj Close: float
- Volume: int
- vol_moving_avg: float
- adj_close_rolling_med: float

# Problem 3: Integrate ML Training

