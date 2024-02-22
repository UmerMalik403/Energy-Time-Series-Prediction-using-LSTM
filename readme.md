**README.md**

# Energy Time Series Prediction using LSTM

## Overview
This repository contains a Python script for time series prediction using Long Short-Term Memory (LSTM) neural networks. The script uses the Keras library with TensorFlow backend for building and training the LSTM model. The dataset used for training and testing is loaded from a CSV file (`energy_train_1d_dirty.csv`), and the predictions are evaluated against the actual values.

## Prerequisites
- Python 3.x
- Required Python libraries: pandas, numpy, matplotlib, scikit-learn, keras, tensorflow, statsmodels

## Instructions

1. **Dataset**
   - The dataset is loaded from the file `energy_train_1d_dirty.csv` using pandas. It is important to ensure that the dataset is in the correct format and has the required columns.

2. **Data Exploration**
   - The script includes data exploration steps, such as plotting time series data and autocorrelation function (ACF) plots.

3. **Data Preprocessing**
   - The dataset is preprocessed by handling missing values, creating lag features, and scaling the input and output variables.

4. **Model Training**
   - The script trains an LSTM model with varying numbers of neurons. The training and testing losses are plotted for different neuron configurations to help in model selection.

5. **Final Model Training**
   - The final LSTM model is trained with the selected number of neurons and optimized using the Adam optimizer.

6. **Evaluation**
   - The script evaluates the trained model on the test set and visualizes the predictions against the actual values for each target variable (value_max, value_min, value_avg).

7. **Error Analysis**
   - The mean and standard deviation of prediction errors are calculated and printed for each target variable.

## How to Run
1. Clone the repository.
   ```bash
   git clone https://github.com/your-username/energy-time-series-prediction.git
   cd energy-time-series-prediction
   ```

2. Install required dependencies.
   ```bash
   pip install -r requirements.txt
   ```

3. Run the script.
   ```bash
   python energy_prediction_script.py
   ```

4. View the results.
   - Check the generated plots and printed error statistics for model evaluation.

## Notes
- The script assumes that the input dataset is in the specified format and may require modification for different datasets.
- Experiment with hyperparameters, such as the number of neurons and epochs, for better model performance.

Feel free to reach out for any questions or improvements!