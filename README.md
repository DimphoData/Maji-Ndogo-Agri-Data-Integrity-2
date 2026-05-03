Maji Ndogo: Crop Yield Prediction Pipeline 🌾
- Project Overview
This project is an end-to-end data engineering and predictive analytics pipeline developed for the Maji Ndogo agricultural initiative. The goal was to build a robust system that ingests messy field survey data, cleans it using automated scripts, and applies a Linear Regression model to predict crop yield based on environmental factors like rainfall and temperature.

- The Tech Stack

1, Python: Core logic using Pandas and NumPy.

2, SQL: Multi-table joins to consolidate geographic, weather, soil, and management data.

3, Machine Learning: Scikit-Learn for Linear Regression modeling and evaluation.

4, Data Engineering: SQLAlchemy for database ingestion and Regular Expressions (Regex) for sensor data extraction.

- Project Structure
The repository is organized into a modular architecture to ensure scalability and professional-grade code management.

data_ingestion.py: Handles the connection to the SQLite database and executes complex SQL joins.

field_data_processor.py: A modular cleaning engine that uses Regex to standardize messy IoT sensor strings.

validate_data.py: A validation layer to ensure data integrity across the pipeline.

Maji_Ndogo_Yield_Prediction.ipynb: The Master Notebook that executes the full pipeline and trains the regression model.

Maji_Ndogo_farm_survey_small.db: The source database containing over 5,000 unique records.

Data Pipeline & Results
The pipeline transforms raw data into a clean, model-ready format by standardizing weather inputs and resolving data inconsistencies.

1. Feature Correlation
The analysis identified key relationships between environmental variables and crop success.

2. Model Performance
The Linear Regression model predicts Standard_yield by analyzing the impact of Ave_temps, Pollution_level, and Rainfall.

R² Score: 0.0807

RMSE: 0.1107
