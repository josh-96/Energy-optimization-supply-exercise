
# Forecasting and Optimization of Energy Demand Using Machine Learning and Probabilistic Methods

This repository contains a Jupyter Notebook that explores the use of machine learning and probabilistic methods to forecast energy demand and optimize predictions under uncertainty. The notebook demonstrates how different methods adjust machine learning forecasts, showcasing their calibration, robustness, and flexibility under new conditions.

## Project Overview

The project focuses on comparing the performance of various methods for forecasting energy demand, including:

Baseline (LSTM Alone): A recurrent neural network trained to predict energy demand.

Bayesian-Adjusted LSTM: Combines LSTM predictions with Bayesian methods to better account for uncertainty and calibrate forecasts.

Probabilistic Zonotopes: A probabilistic approach that extends zonotopes to manage uncertainty and variability.

Dempster-Shafer Theory (DST): A framework for combining evidence under uncertainty.

DST with Weather Data: DST is extended to incorporate additional evidence from weather data.

Dempster-Shafer Zonotopes (DSZ): A robust method combining Dempster-Shafer theory with zonotopes for handling high uncertainty.


The notebook also compares these methods using metrics like forecasted capacity (TWh) and mean costs (€).

## Repository Contents

Notebook: The primary notebook (optimization_energy_production.ipynb) containing all code, visualizations, and analyses.

Graphs and Visualizations: Includes bar plots comparing forecasted capacities and costs across methods.

Sample Data: The dataset used for training and testing the models.

Results and Observations: Insights derived from the analysis and a detailed discussion on the performance of each method.


## Methods and Insights

Baseline (LSTM Alone): The most conservative approach, capturing general patterns but lacking adjustments for variability and external factors.

Bayesian Adjustment: Significantly improves calibration, reducing overestimation by leveraging uncertainty modeling.

Probabilistic Zonotopes: Strikes a balance between over- and underfitting, demonstrating adaptability and conservatism.

DST with Weather Data: Provides the most reduced forecasts, potentially due to seasonal adjustments and weather correlations.

Dempster-Shafer Zonotopes: The most conservative adjusted method, demonstrating resilience and robustness under high uncertainty.


## Key Findings

Bayesian methods successfully recalibrate forecasts without overfitting, especially when applied to unseen test data.

Probabilistic zonotopes provide a balanced approach that accounts for variability while avoiding extremes.

DST with weather data showcases the influence of external factors, emphasizing the importance of data quality and relevance.

DSZ demonstrates robust forecasting in the presence of high uncertainty, making it ideal for critical scenarios.


## Getting Started

Prerequisites

To run the notebook, you need:

Python 3.8 or later

Jupyter Notebook or JupyterLab

Required libraries (install with pip):

numpy

pandas

matplotlib

scikit-learn

pyomo

## How to Run

1. Clone the repository:

git clone https://github.com/yourusername/forecasting-optimization-energy.git
cd forecasting-optimization-energy

2. Open the Jupyter Notebook:

jupyter notebook optimization_energy_supply.ipynb


3. Run all cells in the notebook to reproduce the results and visualizations.

## Visualizations

Data distribution

Bayesian Adjustment

Dempster-Shafer rule of combination 

Dempster-Shafer Zonotope bounds

Forecasted Capacities

Mean Costs

## Future Work

Test the methods on larger and more diverse datasets for better generalization.

Integrate more external factors (e.g., economic data, real-time demand fluctuations) into the forecasts.

Optimize the computational efficiency of probabilistic methods for real-time applications.


## Contributing

Contributions are welcome! Feel free to fork this repository, submit issues, or create pull requests.

