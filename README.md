# Data Cleaning and LSTM Prediction

This Jupyter Notebook contains code for cleaning data and building an LSTM (Long Short-Term Memory) model for predicting the housing index into 2021 (last updated dataset). The code is written in Python and utilizes several libraries, including NumPy, Matplotlib, Pandas, and scikit-learn.

## Cleaning Data

The first part of the notebook focuses on cleaning the data before training the LSTM model. The following steps are performed:

1. Importing the necessary libraries for data cleaning, data plotting, data ingestion, and data preprocessing.
2. Reading the data from the 'data.csv' file using Pandas.
3. Splitting the data into training and test sets based on a specific date.
4. Cleaning the training data by dropping unnecessary columns ('REF_DATE' and 'GEO') and keeping only the 'VALUE' column for prediction.
5. Applying MinMax scaling to normalize the training data.

## Building LSTM

The second part of the notebook focuses on building the LSTM model. The steps involved are as follows:

1. Importing the required libraries for building the LSTM model, including Sequential, Dense, LSTM, and Dropout from the TensorFlow Keras module.
2. Defining the architecture of the LSTM model by adding multiple LSTM layers with dropout regularization.
3. Compiling the LSTM model with the 'adam' optimizer and the mean squared error loss function.
4. Training the LSTM model using the training data.
5. Evaluating the trained LSTM model by preparing the test dataset and making predictions.
6. Performing inverse scaling to bring the predicted values back to the original scale.
7. Visualizing the predicted values along with the actual values using Matplotlib.

## Prerequisites

Before running the code in this notebook, ensure that the following libraries are installed:

- NumPy
- Matplotlib
- Pandas
- scikit-learn
- TensorFlow

Also, make sure that the 'data.csv' file is present in the same directory as this notebook.

## Usage

1. Open visualization_source using JupyterLab, Jupyter Notebook, or any compatible environment.
2. Make sure the required libraries and the dataset ('data.csv') are available.
3. Run each code cell sequentially to perform data cleaning, build the LSTM model, and visualize the predictions.

Note: Adjustments may be required based on specific dataset characteristics or model requirements.

