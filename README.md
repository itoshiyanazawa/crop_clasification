# Crop Selection with Machine Learning

## Project Overview

This project uses machine learning techniques to help farmers select the best crops for their fields based on soil conditions. By analyzing key soil metrics such as nitrogen, phosphorous, potassium levels, and pH value, we can predict the optimal crop choice to maximize yield.

## Dataset

The dataset (`soil_measures.csv`) contains the following features:

- "N": Nitrogen content ratio in the soil
- "P": Phosphorous content ratio in the soil
- "K": Potassium content ratio in the soil
- "pH": pH value of the soil
- "crop": Target variable (categorical) representing various crops

Each row in the dataset represents soil measurements for a particular field, with the "crop" column indicating the optimal choice for that field.

## Methodology

We use XGBoost, a powerful gradient boosting algorithm, to build a multi-class classification model. The project involves the following steps:

1. Data preprocessing and splitting into training and test sets
2. Initial model training and feature importance analysis
3. Hyperparameter tuning using random search
4. Final model evaluation and selection

## Key Findings

- The most important feature for predicting the optimal crop is potassium (K) content in the soil.
- The best model achieved an accuracy of 83.03% on the test set.
- Optimal hyperparameters were found through random search.

## Requirements

- Python 3.x
- pandas
- scikit-learn
- xgboost
- matplotlib
- numpy
- scipy

## Usage

1. Clone the repository
2. Run the Jupyter notebook or Python script to train and evaluate the model

## Future Improvements

- Incorporate additional soil and environmental features
- Experiment with other machine learning algorithms
- Develop a user-friendly interface for farmers to input their soil data and receive crop recommendations

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.
