Impact of AI on Major Technology Stocks

## Project Overview

This project analyzes the impact of the AI boom on major technology stocks:

- NVIDIA (NVDA)
- Microsoft (MSFT)
- AMD (AMD)
- NASDAQ Composite (^IXIC)

The objective is to clean financial market data, perform exploratory visualization, and derive insights from stock performance trends. The repository also includes a predictive modeling workflow that uses the cleaned data to compare three classifiers on the same feature set.

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

## Task 2 Objectives

- Build a predictive modeling dataset from the cleaned market data
- Engineer lagged and rolling features for time-series style modeling
- Compare Logistic Regression, Decision Tree, and Random Forest models
- Export model comparison metrics and feature importance results

## Tools Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- yfinance
- scikit-learn

## Visualizations

See the `reports/data_cleaning_visualization/figures` folder for generated PNGs (01_close_price_trend.png, 02_normalized_close.png, ...).

Predictive modeling outputs are saved in `reports/predictive_modeling/`:

- `model_comparison_results.csv`
- `feature_importance.csv`

## Repository Structure

- data/: raw and cleaned CSVs
- notebooks/: analysis notebooks (`DataCleaning&Visualization.ipynb`, `PredictiveModeling.ipynb`)
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

3. Open `notebooks/DataCleaning&Visualization.ipynb` to reproduce the cleaning and visualization workflow.

4. Open `notebooks/PredictiveModeling.ipynb` to reproduce the modeling workflow and regenerate the results in `reports/predictive_modeling/`.

## Notes

- The raw data downloaded via `yfinance` is stored in `data/ai_stocks_raw.csv`.
- Cleaned dataset and summary CSVs are saved under `reports/data_cleaning_visualization/` and `data/cleaned_ai_stocks_task1.csv`.
- Predictive modeling metrics and feature rankings are saved under `reports/predictive_modeling/`.

## Author

Bishnu Prasad Kar
