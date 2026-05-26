Impact of AI on Major Technology Stocks

## Project Overview

This project analyzes the impact of the AI boom on major technology stocks:

- NVIDIA (NVDA)
- Microsoft (MSFT)
- AMD (AMD)
- NASDAQ Composite (^IXIC)

The objective is to clean financial market data, perform exploratory visualization, and derive insights from stock performance trends.

## Dataset

Source: Yahoo Finance

Period: 2018-2026

## Task 1 Objectives

- Missing value treatment
- Duplicate removal
- Outlier handling
- Feature engineering
- Data visualization
- Dashboard creation

## Tools Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- yfinance

## Visualizations

See the `reports/data_cleaning_visualization/figures` folder for generated PNGs (01_close_price_trend.png, 02_normalized_close.png, ...).

## Repository Structure

- data/: raw and cleaned CSVs
- notebooks/: analysis notebooks (DataCleaning&Visualization.ipynb)
- reports/: generated figures and CSV summaries
- models/: (currently empty)

## How to run

1. Create a virtual environment (recommended):

```bash
python -m venv .venv
source .venv/bin/activate   # or .venv\Scripts\activate on Windows
```

2. Install dependencies:

```bash
pip install -r requirements.txt
```

3. Open the notebook `notebooks/DataCleaning&Visualization.ipynb` and run the cells (or execute as a script after adapting paths).

## Notes

- The raw data downloaded via `yfinance` is stored in `data/ai_stocks_raw.csv`.
- Cleaned dataset and summary CSVs are saved under `reports/data_cleaning_visualization/` and `data/cleaned_ai_stocks_task1.csv`.

## Author

Bishnu Prasad Kar
