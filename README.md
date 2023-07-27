# Sepsis Prediction using LSTM

This repository contains code for predicting sepsis occurrence using an LSTM-based deep learning model. The goal is to predict the occurrence of sepsis using time series data from multiple patients, using the [PhysioNet/Computing in Cardiology Challenge 2019 Dataset](https://physionet.org/content/challenge-2019/1.0.0/).

## Installation
1) Clone the repository:

    git clone https://github.com/msplittgerber/sepsis-shock-prediction.git

2) Explore the Jupyter notebook in the repository:
   Covers the preprocessing steps for handling missing values, feature engineering, and scaling the data.
   Includes feature selection using xgboost.
   Includes the implementation of the LSTM model and training process.
   Evaluates the trained model on the test set and computes performance metrics.
   
3) Modify the code and experiment with different parameters as needed.


## Results

The LSTMs show promising results in predicting sepsis occurrence based on time-series data. Overall, increasing the window size from 5 to 10 resulted in improved accuracy, precision, recall, and AUROC scores. The model with a window size of 10 performed better in terms of correctly predicting positive cases (higher recall) and had a higher precision. However, the overall performance of both models can still be considered moderate, and further refinement and optimization may be required to achieve better results.

## Outlook
For future research, it is essential to validate the model on larger prediction horizons (> 1 hour into the future) and diverse datasets to assess its generalizability. Additionally, exploring other deep learning architectures, such as attention-based models, and incorporating additional contextual information could further enhance the prediction performance.
