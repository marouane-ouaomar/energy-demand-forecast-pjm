# Energy Demand Forecasting (PJM / EIA Dataset)

A data science project focused on analyzing and forecasting electricity demand using PJM energy data.  
The project covers data cleaning, feature engineering, time series analysis, and forecasting models.

---

## Objective

- Analyze electricity demand patterns over time  
- Engineer time-based features for machine learning  
- Build forecasting models for energy consumption  
- Explore seasonality, trends, and anomalies  

---

## Dataset

The dataset contains hourly energy demand data with:

- Timestamped records  
- Multiple demand categories (e.g., D, DF, NG, TI depending on source)  
- Time series structure for forecasting  

---

## Project Structure


energy-demand-forecast-pjm/
│
├── data/
│ ├── raw/ # Original dataset (not pushed to GitHub)
│ └── processed/ # Cleaned dataset
│
├── notebooks/ # Jupyter notebooks
├── models/ # Trained models
├── dashboard/ # Visualization / BI assets
├── reports/ # Final analysis reports
├── requirements.txt
└── README.md


---

## Setup

### 1. Clone repository

```bash
git clone https://github.com/<your-username>/energy-demand-forecast-pjm.git
cd energy-demand-forecast-pjm

2. Create environment

conda create -n energy python=3.11
conda activate energy

3. Install dependencies
pip install -r requirements.txt

Workflow

1. Data Preparation
Load raw dataset
Handle missing timestamps
Pivot structure into time series format
2. Feature Engineering
Extract hour, day, month
Add seasonality features
Create rolling averages
Apply cyclical encoding (sin/cos)

3. Modeling (planned)
Prophet forecasting
Machine learning regression models
Time series evaluation (MAE, RMSE)
Future Work
Real-time forecasting pipeline
Power BI dashboard integration
API deployment (FastAPI)
Advanced deep learning models (LSTM)
