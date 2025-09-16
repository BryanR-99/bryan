---
layout: default
title: Sales Forecasting
---

# Sales Forecasting (Hierarchical TS)

**Problem.** Forecast weekly sales for 120 SKUs across 12 regions to improve replenishment.

**Data.** 3 years of POS data + promos, holidays, pricing, and weather.

**Approach.**
- Built a **hierarchical** forecasting pipeline (SKU → category → region) with reconciliation.
- Compared **LightGBM**, **Prophet**, and **SARIMAX**; engineered lags/rolling stats and promo features.
- Automated backtesting with time-based CV and MLflow tracking.

**Results.**
- MAPE ↓ **12.7%** vs baseline; stockouts ↓ **9.3%**; overstocks ↓ **6.1%**.
- Delivered **dbt** models + scheduled **Airflow** jobs; dashboard in **Plotly Dash**.

**Links.**
- Code: <https://github.com/YOUR_GH/sales-forecasting>
- Dashboard: <https://your-dash-app.example.com>
- Back to [Home](/)