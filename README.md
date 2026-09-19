# EV Dynamic Pricing

An AI-based smart EV charging system that predicts charging prices dynamically based on charging demand, power consumption, grid load, and time-related factors.

## Overview

The project implements a machine learning-based dynamic pricing system for electric vehicle (EV) charging. The system uses charging and grid-related parameters to predict the charging price in ₹/kWh.

A Random Forest Regression model is trained on EV charging data and integrated with an interactive Streamlit dashboard for real-time price prediction and charging recommendations.

## Key Features

- Dynamic EV charging price prediction
- Machine learning-based pricing using Random Forest Regression
- Dataset generation and preprocessing
- Feature-based demand and grid-load analysis
- Model evaluation using MAE, MSE, and R² score
- Feature importance analysis
- Interactive Streamlit dashboard
- Charging-period recommendations based on predicted price
- Visualization of system and charging parameters

## System Workflow

```text
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
Input Parameters

The prediction model uses parameters related to EV charging and grid conditions, including:

Time of day
Voltage
Current
Power factor
Power consumption
Energy consumption
Cumulative energy
Demand level
Grid load
Peak-hour status
Machine Learning Model

The project uses a Random Forest Regressor to predict the charging price.

The dataset is divided into training and testing sets, followed by model training and evaluation.

Evaluation Metrics

The model is evaluated using:

Mean Absolute Error (MAE)
Mean Squared Error (MSE)
R² Score

Feature importance is also calculated to identify the parameters contributing most to the predicted charging price.

Dashboard

The project includes an interactive Streamlit dashboard that allows users to adjust charging parameters and observe the predicted charging price.

The dashboard displays:

Current charging price
Charging power
Energy consumption
Demand level
Grid load
Peak-hour status
Power utilization
Charging recommendations
Live system calculations

Charging periods are categorized based on the predicted price to indicate relatively lower, moderate, or higher charging-cost periods.

Technologies Used
Python
Pandas
NumPy
Scikit-learn
Random Forest Regression
Joblib
Streamlit
FastAPI
Pydantic
Project Structure
EV-Dynamic-Pricing/
│
├── models/
│   └── pricing_model.pkl
│
├── dashboard.py
├── dataset_generation.py
├── step1_data_preparation.py
├── step2_train_model.py
├── step3_test model.py
├── step4_api_integration.py
├── step5_defining_helper_function.py
├── step6_defining_main_function.py
├── step7_error_calc_evaluation.py
│
├── ev_dynamic_pricing_60days.csv
├── trial_dataset_manually_made.csv
└── requirements.txt
