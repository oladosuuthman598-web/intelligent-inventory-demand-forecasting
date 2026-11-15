# Project Plan: Intelligent Inventory Demand Forecasting

## 1. Background
Inventory decisions depend on estimates of future demand. Forecasts that are too low may contribute to stockouts and lost sales; forecasts that are too high may increase holding costs and working capital requirements. This project applies data science to a practical Industrial and Production Engineering problem.

## 2. Problem statement
Using historical sales observations, investigate how to estimate daily units sold for each product over the next seven days. Forecasts may later be considered as inputs to inventory planning, subject to data quality and operational constraints.

## 3. Project definition
- Granularity: product-level daily observations.
- Forecast horizon: seven days ahead.
- Target: units sold.
- Primary task: time-series demand forecasting.
- Status: initial setup; dataset and model are yet to be finalised.

## 4. Objectives
1. Acquire a suitable, properly licensed historical sales dataset.
2. Understand its structure, quality and limitations.
3. Identify trend, seasonality, calendar effects and product-level behaviour.
4. Establish baseline forecasts.
5. Train and compare appropriate forecasting approaches.
6. Evaluate generalisation using chronological validation.
7. Explain how forecasts could support replenishment decisions.

## 5. Proposed methodology

### Phase A — Data understanding
- Record dataset source, licence, fields and time coverage.
- Check missing dates, duplicates, invalid values and inconsistent product identifiers.
- Determine whether the data represents sales, orders or unconstrained demand estimates.

### Phase B — Exploratory analysis
- Plot daily and weekly demand patterns.
- Examine product-level variability and intermittent demand.
- Investigate trends, seasonality, outliers and calendar effects.
- Document findings and data-quality decisions.

### Phase C — Preparation and baselines
- Sort observations chronologically.
- Define the target and prediction horizon.
- Create lag and calendar features where appropriate.
- Establish simple baselines, such as last-value and seasonal-naive forecasts.

### Phase D — Modelling
- Select models based on dataset characteristics and baseline performance.
- Keep training and evaluation periods chronological.
- Avoid information leakage when creating features and fitting transformations.

### Phase E — Evaluation
Potential metrics:
- **MAE:** average absolute forecast error.
- **RMSE:** gives greater weight to larger errors.
- **WAPE:** total absolute error relative to total actual demand, where the denominator is non-zero.

Compare models against a baseline and report results by product or demand segment where useful.

### Phase F — Inventory interpretation
Explore how forecasts could inform replenishment. Reorder-point or safety-stock calculations require additional inputs and assumptions, such as lead time, service level and lead-time demand variability.

## 6. Important limitation
Recorded sales can be lower than actual customer demand during stockouts. If stock-availability data is unavailable, do not treat every observed sales value as an unquestionable measure of true demand.

## 7. Deliverables
- Documented dataset source and data dictionary.
- Exploratory analysis notebook.
- Reproducible preparation and modelling code.
- Baseline and model evaluation.
- Forecast examples and interpretation.
- Final project report and updated README.

## 8. Progress log

| Stage | Status |
|---|---|
| Project idea and scope | Defined |
| GitHub repository setup | In progress |
| Dataset selection | Pending |
| Data cleaning and EDA | Pending |
| Baseline forecasting | Pending |
| Model development | Pending |
| Evaluation and interpretation | Pending |
| Final documentation | Pending |
