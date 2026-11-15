# Intelligent Inventory Demand Forecasting

An applied data science and machine learning project exploring how historical sales data can support better inventory planning.

## Project overview
Retailers need to estimate future demand to make informed replenishment decisions. Underestimating demand can contribute to stockouts, lost sales and customer dissatisfaction; overestimating it can increase holding costs and tie up working capital.

This project investigates **product-level daily demand forecasting** and a forecast horizon of the **next 7 days**.

## Objectives
- Explore historical sales and identify demand patterns.
- Prepare time-series data for modelling.
- Forecast daily units sold for the next seven days.
- Evaluate forecasts with time-aware validation and suitable error metrics.
- Discuss how forecasts could inform inventory and replenishment decisions.

## Current scope

| Item | Definition |
|---|---|
| Forecasting level | Product-level, daily |
| Forecast horizon | Next 7 days |
| Target | Units sold |
| Problem | Time-series demand forecasting |
| Status | In progress |

The dataset, final model and model performance have not yet been established. Results will be documented as the work progresses.

## Planned workflow
1. Select and document a suitable historical sales dataset and its licence.
2. Inspect data quality, missing values, duplicates and date coverage.
3. Explore trends, seasonality and product-level variation.
4. Establish simple baseline forecasts.
5. Build and compare suitable forecasting models.
6. Use chronological train/validation/test splits, not random shuffling.
7. Evaluate with metrics such as MAE, RMSE and WAPE where appropriate.
8. Discuss practical implications and limitations for inventory planning.

## Repository structure
```text
├── data/
│   ├── raw/              # Original data (not committed)
│   └── processed/        # Cleaned/intermediate data (not committed)
├── docs/
│   └── project_plan.md
├── notebooks/
├── src/
├── requirements.txt
└── README.md
```

## Getting started
Clone the repository:
```bash
git clone https://github.com/oladosuuthman598-web/intelligent-inventory-demand-forecasting.git
cd intelligent-inventory-demand-forecasting
```

Create and activate a virtual environment:

Windows:
```bash
python -m venv .venv
.venv\Scripts\activate
```

macOS/Linux:
```bash
python -m venv .venv
source .venv/bin/activate
```

Install dependencies and start Jupyter:
```bash
pip install -r requirements.txt
jupyter notebook
```

## Data and reproducibility
No dataset is included yet. Once selected, its source, access date, licence and preparation steps will be documented. Raw and processed data files are excluded from Git by default. Do not commit confidential, personal or restricted data.

## Important limitation
Observed sales are not always the same as true customer demand. During stockouts, recorded sales may understate demand. This limitation will be considered when interpreting the data and forecasts.

## Author
**Oladosu Uthman Bayonle**  
Industrial and Production Engineering | Data Science and Machine Learning

[GitHub profile](https://github.com/oladosuuthman598-web)

---
*Ongoing learning and portfolio project. Documentation will be updated as implementation and evaluation progress.*
