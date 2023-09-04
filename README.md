# COVID-19_Drug_design 

This GitHub repository contains the code and resources for a machine-learning project focused on predicting the inhibition potential of chemical compounds against the COVID-19 virus. The project uses a dataset that consists of IC50 (half-maximal inhibitory concentration) data for 104 chemical molecules.

## Dataset Description

### Original Dataset
- `original_dataset.csv`: The original dataset contains the SMILES notation and pIC50 constant values for chemical compounds. The pIC50 values represent the negative logarithm of the IC50 values, which measure the potency of compounds against the COVID-19 virus.

### Engineered Features Dataset
- `engineered_features_dataset.csv`: In this file, features were generated using the PubChemPy library in Python. These engineered features provide additional chemical information that can enhance the predictive power of machine learning models.

## Project Structure

The repository is organized as follows:

- `data/`: This directory contains the dataset files.
- `Notebook`: Jupyter notebook used for data preprocessing, model development, and evaluation.
- `README.md`: This README file provides an overview of the project and repository.

## Usage

To reproduce the results or further develop this project:

1. Clone this repository to your local machine.

3. Explore the Jupyter Notebook for data preprocessing, model development, and evaluation.

4. Use the trained model for predictions or further analysis.

## Results

The results from the model evaluation are as follows:

| Algorithm                  | Mean Squared Error (MSE) | Mean Absolute Error (MAE) | Training Time (s) |
|----------------------------|--------------------------|---------------------------|--------------------|
| SVR                        | 0.188553                 | 0.365123                  | 0.000000           |
| RandomForestRegressor      | 0.221169                 | 0.377919                  | 0.381423           |
| GradientBoostingRegressor  | 0.244222                 | 0.351529                  | 0.140153           |
| KNeighborsRegressor        | 0.245489                 | 0.406286                  | 0.187452           |
| BaggingRegressor           | 0.246224                 | 0.406631                  | 0.028171           |
| SGDRegressor               | 0.342725                 | 0.528698                  | 0.015689           |
| AdaBoostRegressor          | 0.349784                 | 0.513483                  | 0.119014           |
| LinearRegression           | 0.401804                 | 0.445180                  | 0.031387           |
| DecisionTreeRegressor      | 0.650199                 | 0.726470                  | 0.000000           |
| ExtraTreeRegressor         | 0.771604                 | 0.745971                  | 0.015045           |

## Conclusion

This project serves as a starting point for predicting the inhibition potential of chemical compounds against the COVID-19 virus. It provides a comparative analysis of various machine learning algorithms' performance.

Feel free to contribute, modify, or extend this project to improve its accuracy and usability. If you have any questions or suggestions, please create an issue or reach out to the project contributors.
