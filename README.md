# Predictive Analytics for Crime Arrests Using Deep Learning

## Objective
The goal of this project is to leverage deep learning models to predict the likelihood of arrests in crime incidents using temporal and contextual data from the City of Chicago. The study aims to identify patterns that influence arrest outcomes, providing insights for predictive policing and improved resource allocation.

## Key Features
- Implementation of three deep learning models: Convolutional Neural Network (CNN), Recurrent Neural Network (RNN), and Multi-Layer Perceptron (MLP).
- Focus on capturing temporal patterns in crime data to enhance prediction accuracy.
- Comparison of model performance to determine the most effective approach for predicting arrests.
- Preprocessing of crime data, including feature encoding and standardization.
- Visualization of data distributions and correlation analysis for feature selection.

## Data Description
The dataset used in this project is sourced from the Chicago Police Department's Uniform Crime Reporting data. Key attributes include:
- **ARREST**: A binary target variable indicating whether an arrest was made.
- **PRIMARY DESCRIPTION**: The main type of crime (e.g., theft, assault).
- **SECONDARY DESCRIPTION**: A detailed category of the crime.
- **LOCATION DESCRIPTION**: Type of location where the crime occurred.
- **DOMESTIC**: A binary indicator if the crime was domestic-related.
- **Temporal Features**: Information related to the timing of the crime (e.g., time of day, day of the week).
- **Coordinates**: Spatial data including X, Y coordinates and geographic latitude/longitude.

## Project Overview
This project follows a structured methodology to build and evaluate deep learning models:
1. **Data Preprocessing**: Cleaning and encoding of categorical features, standardization of numeric data, and visualization of data distributions.
2. **Model Design**:
   - **CNN**: Captures temporal patterns using convolutional layers.
   - **RNN**: Utilizes sequential patterns with LSTM layers.
   - **MLP**: Applies dense layers for pattern recognition without temporal emphasis.
3. **Training and Evaluation**: Models were trained on an 80-20 train-test split, with accuracy and loss metrics monitored throughout the process.
4. **Comparison**: Performance of each model was compared to identify the best approach for predicting arrests based on the dataset.

## Results
- **CNN Model**: Achieved the highest accuracy of 91.76\%, demonstrating strong performance in identifying key temporal trends influencing arrests.
- **RNN Model**: Reached an accuracy of 89.34\%, effectively capturing sequential patterns in the data.
- **MLP Model**: Scored an accuracy of 87.29\%, highlighting the importance of time-series analysis in arrest prediction.
- The CNN’s superior performance suggests that temporal data plays a crucial role in predicting arrests, making CNN an effective choice for this application.
