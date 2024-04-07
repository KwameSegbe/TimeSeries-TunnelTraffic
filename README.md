# Tunnel Traffic Forecasting Analysis

## Author
Francis Kwame Segbe

## Project Overview
This project aims to predict daily vehicle traffic through a tunnel using historical data. We apply ARIMA, Prophet, and LSTM models to provide actionable insights for traffic management and infrastructure planning.

## Data Description
The dataset spans 747 days of traffic counts, starting from November 1, 2003. It consists of the following attributes:
- **Day**: The date of the traffic count (YYYY-MM-DD).
- **NumVehicles**: The number of vehicles that passed through the tunnel on that day.

## Analytical Approach and Methodology
The project unfolds across multiple phases, each focusing on a distinct aspect of the forecasting challenge:

### Data Preparation
- **Data Import and Exploration**: Employ Pandas for data ingestion and Seaborn for initial visual analysis.

### Time Series Decomposition and Forecasting
- **ARIMA Model**: Select optimal ARIMA parameters based on AIC and use `pmdarima.auto_arima` and `statsmodels.tsa.arima.model` for model execution.
- **Prophet Model**: Leverage Facebook's Prophet for its proficiency with seasonality and holiday effects.
- **LSTM Network**: Employ deep learning to capture complex data patterns, with an emphasis on both short and long-term dependencies.

### Evaluation and Validation
- Apply MSE and RMSE metrics for performance assessment.

## Results
- **ARIMA Model**: Captured linear time series aspects, RMSE: 4030.644.
- **Prophet Model**: Exhibited improved accuracy with seasonal handling, RMSE: 2383.947.
- **LSTM Model**: Outperformed other models in complexity management, RMSE: 2169.473.

## Discussion and Insights
Our findings reveal the strengths of combining statistical and machine learning methods for forecasting. The LSTM model, in particular, shows high potential in managing the temporal dynamics inherent in traffic data.

## Recommendations for Future Work
- **Data Enrichment**: Integrate weather conditions, holidays, and event data.
- **Model Exploration**: Test hybrid and advanced neural network architectures like GRU.
- **Deployment Strategy**: Establish a real-time forecasting and model updating pipeline.

## Conclusion
This analysis provided a nuanced understanding of traffic patterns and model efficacy in forecasting. The continued refinement and data expansion will further improve forecast precision, thus enhancing tunnel traffic management and planning.

## How to Use
1. Clone the repository.
2. Install the required libraries listed in `requirements.txt`.
3. Run the Jupyter Notebooks to replicate the analysis.

## Contributions
Contributions to improve the models or explore new data sources are welcome. Please submit a pull request or open an issue to discuss your ideas.

## License
The analysis is open-sourced under the MIT License. See `LICENSE` for more information.

## Contact
For inquiries or collaboration offers, please reach out to [Francis Kwame Segbe](mailto:francis.segbewb@email.com).
