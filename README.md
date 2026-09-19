#EV Dynamic Pricing

An AI-based smart EV charging system that predicts charging prices dynamically based on charging demand, power consumption, grid load, and time-related factors.

Overview

This project implements a machine learning-based dynamic pricing system for electric vehicle (EV) charging. The system uses charging and grid-related parameters to predict the charging price in ₹/kWh.

A Random Forest Regression model is trained on EV charging data and integrated with an interactive Streamlit dashboard for dynamic price prediction and charging recommendations.

Key Features
Dynamic EV charging price prediction
Machine learning-based pricing using Random Forest Regression
Dataset generation and preprocessing
Charging demand and grid-load analysis
Model evaluation using MAE, MSE, and R² score
Feature importance analysis
Interactive Streamlit dashboard
Charging-period recommendations based on predicted price
Visualization of charging and grid parameters
System Workflow
Dataset Generation
        ↓
Data Preparation
        ↓
Feature Selection
        ↓
Random Forest Model Training
        ↓
Model Testing & Evaluation
        ↓
API Integration
        ↓
Interactive Streamlit Dashboard
        ↓
Dynamic Price Prediction

## Machine Learning Model

The project uses a **Random Forest Regressor** to predict the EV charging price.

The model is trained using charging and grid-related parameters and evaluated on a separate test dataset.

### Evaluation Metrics

The model performance is evaluated using:

- Mean Absolute Error (MAE)
- Mean Squared Error (MSE)
- R² Score

Feature importance analysis is also used to understand which input parameters have the greatest influence on the predicted charging price.
## Dashboard

The project includes an interactive **Streamlit dashboard** for dynamic EV charging price prediction.

The dashboard allows users to provide charging and grid-related parameters and view the predicted charging price.

It displays:

- Predicted charging price
- Charging power
- Energy consumption
- Demand level
- Grid load
- Peak-hour status
- Power utilization
- Charging recommendations

The dashboard provides a simple interface for understanding how charging and grid conditions affect the predicted EV charging price.
