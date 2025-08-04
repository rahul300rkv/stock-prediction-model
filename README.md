# stock-prediction-model
Stock Price Prediction with Deep Learning
Overview
This project implements a stock price prediction system using advanced deep learning techniques such as GRU, LSTM, Conv1D, and Dense neural networks. The system leverages financial technical indicators and performs classification and regression tasks to predict future stock prices and their directional movements.

Features
Data fetching from Yahoo Finance

Calculation of multiple technical indicators (RSI, MACD, ADX, Bollinger Bands, etc.)

Custom loss function combining regression error with directional accuracy

Flexible choice of models: GRU, LSTM, Conv1D, Dense, with optional bidirectional layers

Model training with TimeSeries cross-validation and early stopping

Detailed evaluation metrics: MAPE, RMSE, Directional Accuracy

Interactive Jupyter-based UI for easy experimentation (ipywidgets required)

Saves and loads models automatically with versioning based on training date

Installation
bash
pip install -r requirements.txt
Usage
Run the main script to start the interactive UI (if Jupyter and ipywidgets are available):

bash
python your_script.py
Alternatively, use the train_and_test() or train_or_load_models() functions directly to train models and make predictions.

File Structure
your_script.py: Main Python script containing data processing, model definitions, training, and evaluation

models/: Directory for storing trained models

data/: (Optional) Folder for storing downloaded or processed data files

requirements.txt: Python dependencies for the project

Key Functions
load_data(): Downloads stock data and computes features and labels

add_indicators(): Adds technical indicators to the data

build_model(): Constructs neural network models based on type and bidirectionality

train_and_test(): Trains models using time series cross-validation and evaluates performance

predict_and_evaluate(): Makes predictions with trained models and plots results

Requirements
Python 3.7+

numpy, pandas, matplotlib, scikit-learn

tensorflow (2.x)

yfinance

ipywidgets (optional, for interactive UI)

ta (technical analysis library)
