# Exploratory Data Analysis (EDA) – Revenue Analysis

## Project Overview
This project performs an exploratory data analysis (EDA) on transactional data to understand revenue behavior, data quality, and distribution patterns.  
The analysis focuses on revenue aggregation, temporal trends, and the effect of data preprocessing such as winsorization.

---

## Project Structure
WEEK2/
│
├── data/
│   ├── raw/
│   └── processed/
│       ├── analytics_table.parquet
│       ├── orders_clean.parquet
│       └── users.parquet
│
├── notebooks/
│   └── eda.ipynb
│
├── reports/
│   └── figures/
│       ├── revenue_by_country.png
│       ├── revenue_trend_monthly.png
│       ├── amount_hist_winsor.png
│
├── src/
│   └── bootcamp/
│       ├── io.py
│       ├── joins.py
│       ├── quality.py
│       └── transforms.py
│
├── requirements.txt
└── README.md

---

## Setup Instructions

1. *Create a virtual environment*
```bash
python -m venv .venv

2.	Activate the environment

	•	Windows:
    .venv\Scripts\activate
    •	macOS / Linux:
    source .venv/bin/activate

3.	Install required packages:
pip install -r requirements.txt

## How to Run the Analysis:

1.	Open the notebook:
notebooks/eda.ipynb
2.	Run all cells from top to bottom.
	3.	Generated figures will be automatically saved in:
    reports/figures/

Generated Figures & Insights

1. Revenue by Country

This chart shows total revenue aggregated by country across all transactions.
It highlights which countries contribute the most to overall revenue and helps identify dominant markets.

⸻

2. Revenue Over Time (Monthly)

This line chart visualizes monthly revenue trends.
It helps identify seasonality, growth patterns, and periods of decline or recovery over time.

⸻

3. Order Amount Distribution (Winsorized)

This histogram shows the distribution of order amounts after applying winsorization.
Winsorization reduces the impact of extreme outliers and provides a clearer view of the typical order size distribution.

⸻

Notes
	•	All figures are saved programmatically using Pathlib to ensure portability across different machines.
	•	No absolute file paths are used.
	•	The project is reproducible by following the setup steps above.