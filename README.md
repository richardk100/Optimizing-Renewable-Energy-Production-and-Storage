# Optimizing-Renewable-Energy-Production-and-Storage
This project involves optimizing the energy production and storage for a renewable energy system using solar and wind power. The optimization aims to minimize the total cost while meeting the energy demand over a specific period.

## Project Overview

The system parameters and constraints include the costs associated with solar, wind, and storage capacities, as well as their respective maximum capacities. The optimization is performed using the `scipy.optimize.minimize` function.

## Data

The project utilizes two main datasets:
- `weather_data.csv`: Contains solar irradiance and wind speed data.
- `demand_data.csv`: Contains the energy demand data.

## System Parameters and Constraints

- `COST_SOLAR`: Cost of solar energy per kWh ($0.12).
- `COST_WIND`: Cost of wind energy per kWh ($0.10).
- `COST_STORAGE`: Cost of energy storage per kWh ($0.05).
- `MAX_SOLAR_CAPACITY`: Maximum solar capacity (100 kWh).
- `MAX_WIND_CAPACITY`: Maximum wind capacity (150 kWh).
- `STORAGE_CAPACITY`: Storage capacity (200 kWh).

## Optimization

The objective function for the optimization calculates the total cost based on the solar and wind energy production, storage usage, and energy deficit. The optimization is performed using the `minimize` function from the `scipy.optimize` module with specific bounds for the variables.

## Visualization

The results are visualized using a bar chart for solar, wind, and storage energy production, and a line chart for energy demand.

## How to Run the Project

1. Install the required libraries:
   ```sh
   pip install pandas numpy scipy matplotlib
