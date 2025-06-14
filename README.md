Stock Price Prediction using LSTM

This project demonstrates how to build and train a Long Short-Term Memory (LSTM) neural network to predict stock prices using historical time series data. The implementation is done in a Jupyter Notebook, and the focus is on learning the application of LSTM to financial data forecasting.

Project Objective

To predict future stock prices based on past closing price data using an LSTM model. The aim is to apply LSTM to understand how well it can capture time-dependent trends in stock market data.

Dataset
	•	The dataset used contains historical stock price data in .csv format.
	•	It includes standard columns such as Date, Open, High, Low, Close, and Volume.
	•	Only the closing price is used for modeling.

Workflow
	1.	Data Preprocessing
	•	Loading the CSV file and selecting the Close price column.
	•	Scaling the data using MinMaxScaler.
	•	Splitting the data into training and testing sets (65%-35% split).
	•	Creating a sliding window of 100 time steps for input sequences.
	2.	Model Building
	•	Constructed an LSTM model using Keras.
	•	Layers used: LSTM, Dense.
	•	Compiled using mean squared error loss and Adam optimizer.
	3.	Model Training
	•	Trained the model on the training data.
	•	Evaluated performance on the test set using RMSE.
	4.	Prediction and Visualization
	•	Made predictions on training and test data.
	•	Predicted the next 30 days using recursive forecasting.
	•	Plotted original data along with train and test predictions.

Requirements
	•	Python 3.x
	•	TensorFlow / Keras
	•	NumPy
	•	Pandas
	•	Matplotlib
	•	Scikit-learn

Future Improvements
	•	Add evaluation metrics such as R² score and MAE.
	•	Experiment with different LSTM architectures and dropout regularization.
	•	Add a Streamlit interface for user interaction.
	•	Use live data from financial APIs like Yahoo Finance or Alpha Vantage.
