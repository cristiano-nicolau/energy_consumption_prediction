# Energy Consumption Prediction

## Project Objective
This project aims to predict the energy consumption of buildings using data provided by the [ASHRAE - Great Energy Predictor III](https://www.kaggle.com/competitions/ashrae-energy-prediction/overview) competition on Kaggle.

Accurate energy consumption predictions are essential for optimizing energy efficiency, reducing operational costs, and minimizing environmental impact.

## About the Dataset
The dataset is provided by ASHRAE (American Society of Heating, Refrigerating and Air-Conditioning Engineers) and contains energy consumption measurements from commercial and institutional buildings across various locations. The dataset includes:

- **Energy consumption measurements** (`meter_reading`)
- **Building characteristics**, such as area, construction year, and primary use
- **Weather data**, including air temperature, humidity, wind speed, and more

### Dataset Structure

#### **train.csv** (Training Data)
| Column              | Description |
|---------------------|-------------|
| `building_id`       | Unique identifier for the building |
| `timestamp`         | Date and time of the measurement |
| `meter_reading`     | Measured energy consumption |
| `site_id`           | Identifier for the site |
| `primary_use`       | Primary use of the building (e.g., office, school, hospital) |
| `square_feet`       | Total area of the building |
| `year_built`        | Year the building was constructed |
| `floor_count`       | Number of floors in the building |

#### **weather_train.csv** (Weather Data for Training)
| Column              | Description |
|---------------------|-------------|
| `site_id`           | Identifier for the site |
| `timestamp`         | Date and time of the measurement |
| `air_temperature`   | Air temperature |
| `cloud_coverage`    | Cloud coverage |
| `dew_temperature`   | Dew point temperature |
| `precip_depth_1_hr` | Precipitation (rain/snow) depth per hour |
| `sea_level_pressure`| Atmospheric pressure at sea level |
| `wind_direction`    | Wind direction |
| `wind_speed`        | Wind speed |

## Initial Project Goal
The primary goal is to develop a predictive model capable of estimating **energy consumption (`meter_reading`)** for buildings based on their characteristics and weather conditions.

Key steps include:
- **Data exploration and cleaning** (handling missing values and outliers)
- **Feature selection** to identify relevant predictors
- **Training predictive models** (Random Forest,  FNN, LSTM)
- **Model performance evaluation** using metrics such as RMSLE, MSE, MAE, R2

## References
- [ASHRAE Competition on Kaggle](https://www.kaggle.com/competitions/ashrae-energy-prediction/overview)
