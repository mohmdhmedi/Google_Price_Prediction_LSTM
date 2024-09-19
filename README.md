# Google Stock Price Prediction with EMAs and Candlestick Visualization

## Project Overview

This repository focuses on predicting Google stock prices using historical data and various Exponential Moving Averages (EMAs) over different time periods (9, 21, and 30 days). The project combines machine learning models with advanced data visualization techniques such as candlestick charts to provide insightful visual analyses of predicted and actual stock prices.

Key features:
- **EMA Modeling**: Models built for 9-day, 21-day, and 30-day EMAs.
- **Candlestick Visualization**: Integration of candlestick charts for visualizing actual stock prices.
- **Prediction Analysis**: Comparison of predicted stock prices across different EMAs.
- **Interactive Visualizations**: Utilizes Plotly for dynamic plots and Matplotlib for static analysis.

## Table of Contents
1. [Installation](#installation)
2. [Data](#data)
3. [Modeling Approach](#modeling-approach)
4. [Visualizations](#visualizations)
5. [Results](#results)
6. [Future Work](#future-work)
7. [Contributions](#contributions)
8. [License](#license)

## Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/yourusername/google-stock-price-prediction.git
    ```

2. Install required packages:
    ```bash
    pip install -r requirements.txt
    ```

3. If using Jupyter Notebooks, you can also install Jupyter:
    ```bash
    pip install jupyter
    ```

## Data

The data used in this project includes historical Google stock price information, including features like:
- **Open**
- **High**
- **Low**
- **Close**
- **Volume**

The data is preprocessed and split into training, validation, and test sets. Key preprocessing steps involve:
- Normalizing the data.
- Creating EMA features for 9, 21, and 30 days.

## Modeling Approach

The project builds neural network models using **PyTorch** to predict future stock prices based on:
- 9-day, 21-day, and 30-day EMAs.
- A combined model that integrates all EMAs for holistic predictions.

### Models:
1. **Neural Network Architecture**: A simple fully connected neural network with several layers optimized using Adam optimizer and MSE loss.
2. **Training**: Models are trained for 100 epochs, and the best model is saved based on validation loss.
3. **Evaluation**: Evaluation of models on unseen test data.

## Visualizations

The repository includes multiple visualization tools:
- **Candlestick charts**: Provides a financial charting tool to visualize stock price movements.
- **Predictions**: Overlays predicted stock prices on top of actual prices.
  
Two types of visualizations:
1. **Matplotlib** for static plots.
2. **Plotly** for interactive charts including candlestick visualizations with predictions overlaid for better analysis.

### Example Code for Visualization:
- **Static Plot**: Uses Matplotlib to compare predictions from multiple EMA models.
- **Interactive Plot**: Uses Plotly to generate an interactive candlestick chart with predicted prices overlaid.

## Results

The models provide reasonably accurate predictions of future stock prices based on the past performance of Google stock and EMA indicators. The combined EMA model improves predictive accuracy compared to individual EMAs.

## Future Work

- **Feature Engineering**: Adding more technical indicators (e.g., RSI, MACD).
- **Deep Learning Models**: Experimenting with LSTMs and transformers for time-series prediction.
- **Portfolio Optimization**: Using the predicted prices for investment strategies.
  
## Contributions

Contributions are welcome! Feel free to open an issue or submit a pull request.

## License

This project is licensed under the MIT License.
