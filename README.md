# Model Agnostic Methods Analysis

![](images/12.jpg)

**Prepared for**: UPV Renting Bike .SA\
**Prepared by**: Adrián Tallec de León, Jezabel Esbrí Rodríguez, Manuel Rocamora Valenti

## Introduction

This project aims to apply model agnostic methods to understand the influence of various factors on predicted outcomes. Specifically, we utilize Partial Dependence Plots (PDPs) and Bidimensional Partial Dependency Plots to visualize the relationships learned by Random Forest models. The analysis focuses on predicting bike rental counts and house prices based on key features.

## Project Structure

-   **data/**: Contains the dataset `kc_house_data.csv`.
-   **scripts/**: Contains R scripts for data processing, model training, and plotting.
-   **plots/**: Contains generated plots for analysis.
-   **README.md**: This file.

## Dataset

1.  The dataset `kc_house_data.csv` contains the following features:

-   `id`
-   `date`
-   `price`
-   `bedrooms`
-   `bathrooms`
-   `sqft_living`
-   `sqft_lot`
-   `floors`
-   `waterfront`
-   `view`
-   `condition`
-   `grade`
-   `sqft_above`
-   `sqft_basement`
-   `yr_built`
-   `yr_renovated`
-   `zipcode`
-   `lat`
-   `long`
-   `sqft_living15`
-   `sqft_lot15`

2.  The dataset `day.csv` contains the following features:

-   `days_since_2011`: Number of days since the start of 2011 (potentially a time variable).
-   `temperature`: Temperature on a given day.
-   `humidity`: Humidity level on a given day.
-   `wind_speed`: Wind speed on a given day.
-   `bike_rental_counts`: Number of bikes rented on that day (target variable).

## Analysis

### Partial Dependence Plot

We analyze the influence of key environmental and temporal variables---days since 2011, temperature, humidity, and wind speed---on predicted bike rental counts using Partial Dependence Plots (PDPs).

### Bidimensional Partial Dependency Plot

We utilize a 2D Partial Dependency Plot with a Density Overlay to analyze the interplay between temperature and humidity and its effect on bike rental patterns.

### House Price Prediction

We use a Random Forest model to predict house prices based on features: bedrooms, bathrooms, square footage of living space (sqft_living), and the number of floors. PDPs are used to visualize the relationships between these features and house prices.

## Setup and Installation

**Clone the repository**: `bash git clone https://github.com/MRocVal/miApp.git cd your-repository`
