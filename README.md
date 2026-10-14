# Urban Ride Demand Forecasting & Mobility Analytics

An end-to-end data science project exploring urban taxi demand patterns and forecasting hourly demand across selected New York City Yellow Taxi pickup zones using machine learning and Power BI.

## Project Overview

Urban transportation demand varies by hour and location. Understanding these patterns can help identify busy periods, compare pickup zones, and support data-informed mobility planning.

This project analyzes NYC Yellow Taxi trip data from January to March 2025. It combines data preprocessing, feature engineering, Random Forest forecasting, model evaluation, and an interactive Power BI dashboard.

## Objectives

- Analyze hourly taxi demand across selected NYC pickup zones.
- Explore demand patterns by hour of day.
- Compare total trip volumes across pickup zones.
- Forecast next-hour demand using a Random Forest model.
- Evaluate model performance against a baseline prediction.
- Present key findings through a Power BI dashboard.

## Dataset

The analysis uses NYC Yellow Taxi trip data for January, February, and March 2025, focusing on 10 selected pickup zones.

The combined hourly demand dataset contains **21,600 rows**, covering hourly observations across the selected zones.

**Total trips represented:** 3,923,992.

## Methodology

1. **Data preprocessing:** Prepare and combine trip data for analysis.
2. **Feature engineering:** Construct features for hourly demand forecasting.
3. **Demand analysis:** Examine hourly patterns and compare pickup-zone volumes.
4. **Model development:** Train Random Forest models to predict next-hour demand.
5. **Evaluation:** Compare predictions with actual demand and a baseline approach.
6. **Visualization:** Build a one-page Power BI dashboard for demand analysis and model evaluation.

## Model Evaluation

The March 2025 evaluation produced the following results:

| Model | MAE | RMSE |
|---|---:|---:|
| Baseline | 44.15 | 64.74 |
| Random Forest — January training data | 27.80 | 43.25 |
| Random Forest — January and February training data | 26.12 | 41.10 |

The January–February Random Forest model achieved a **40.8% reduction in MAE** compared with the baseline.

- **MAE (Mean Absolute Error):** Measures the average absolute difference between actual and predicted demand.
- **RMSE (Root Mean Squared Error):** Measures prediction error while penalizing larger errors more heavily.

Lower values indicate better predictive performance.

## Power BI Dashboard

The dashboard presents:

- Total trip volume.
- Number of selected pickup zones.
- March model MAE.
- MAE reduction compared with the baseline.
- Average taxi demand by hour of day.
- Total trips by pickup zone.
- Actual versus predicted taxi demand.

## Tools & Technologies

- Python
- pandas
- scikit-learn
- Random Forest
- Jupyter Notebook
- Power BI
- CSV and Parquet data formats

## Project Structure

```text
Urban-Ride-Demand-Forecasting/
├── datasets/
├── models/
├── results/
├── notebooks/
├── powerbi/
└── README.md
```

*The folder names above describe the intended organization; the repository structure may be updated as project files are added.*

## Key Takeaways

- Taxi demand varies across hours and pickup zones.
- Comparing actual and predicted demand helps assess forecasting performance.
- The evaluated Random Forest model improved on the baseline according to both MAE and RMSE.

## Future Improvements

- Evaluate forecasting performance across additional zones and time periods.
- Explore alternative forecasting models.
- Improve dashboard interactivity and visual presentation.

---

**Project focus:** Urban Mobility Analytics | Time-Series Analysis | Machine Learning | Business Intelligence
