# Smart City IoT Data Ingestion & Analytics API

## Overview

A Python-based API for ingesting, storing, and analyzing simulated smart-city IoT sensor readings. This project combines REST API development, time-series analytics, and unsupervised machine learning to identify potentially unusual sensor values.

## Features

- **REST API:** Built with FastAPI to ingest and retrieve sensor readings.
- **Data Validation:** Uses Pydantic to validate incoming sensor data.
- **Database:** Stores sensor readings in SQLite.
- **Time-Series Analytics:** Groups timestamped readings into hourly summaries.
- **Machine Learning:** Uses Isolation Forest for anomaly detection.
- **Data Visualization:** Uses Pandas and Matplotlib to explore sensor trends and flagged anomalies.
- **Interactive API Documentation:** Provides endpoint documentation through FastAPI.

## Technology Stack

- Python
- FastAPI
- Pydantic
- SQLite
- Pandas
- Scikit-learn
- Matplotlib
- Requests
- Google Colab

## Sensor Categories

The project simulates readings for five sensor categories:

- Traffic
- Air quality
- Energy
- Parking
- Waste

## How It Works

1. Simulated IoT devices send timestamped sensor readings to the API.
2. The API validates the readings and stores them in SQLite.
3. Analytics endpoints calculate summary statistics and hourly trends.
4. Isolation Forest flags statistically unusual readings.
5. Matplotlib visualizes sensor trends and potential anomalies.

## Running the Project

The project was developed and tested in Google Colab.

1. Open the notebook in Google Colab.
2. Install the required Python packages.
3. Run the API setup and server cells.
4. Generate simulated sensor readings.
5. Test the API endpoints.
6. Run the visualization cells to explore the results.

## Important Limitations

- The sensor data is simulated and does not come from real city sensors.
- Anomaly flags are statistical indicators, not confirmed incidents.
- The current version performs time-series analysis but does not implement forecasting.
- The project is a prototype and is not configured for production deployment.

## Future Improvements

- Add automated API tests.
- Evaluate anomaly detection using labelled test data.
- Build an interactive sensor-monitoring dashboard.
- Integrate a real IoT data source.
- Explore time-series forecasting using suitable data.

## Author

MSc Data Science Student
