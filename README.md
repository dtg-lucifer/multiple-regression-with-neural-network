# Bike Sharing Demand Prediction with Linear Regression

## Project Overview

This project demonstrates the application of regression techniques to predict bike sharing demand in Seoul, South Korea based on various environmental factors. The analysis explores both traditional linear regression and neural network approaches to compare their effectiveness in predicting the number of bikes rented based on weather conditions.

## Dataset

The analysis uses the "Seoul Bike Sharing Demand" dataset from the UCI Machine Learning Repository. The dataset contains hourly records of:

- Bike rental counts
- Temperature (°C)
- Humidity (%)
- Wind speed (m/s)
- Visibility (10m)
- Dew point temperature (°C)
- Solar radiation (MJ/m2)
- Rainfall (mm)
- Snowfall (cm)
- Seasons
- Holiday information
- Functioning day status

**Source**: Seoul Bike Sharing Demand [dataset]. 2020. UCI Machine Learning Repository.  
**Available from**: https://doi.org/10.24432/C5F62R

## Project Structure

```
├── data/
│   └── bike_data.csv       # The Seoul bike sharing dataset
├── linear_regression.ipynb # Main analysis notebook
└── README.md               # Project documentation
```

## Installation and Setup

To run this project, you need Python with the following packages:

```bash
pip install numpy pandas matplotlib seaborn scikit-learn tensorflow imblearn
```

## Analysis Approach

The analysis proceeds through several stages:

1. **Data Preparation**:
   - Loading and cleaning the dataset
   - Focus on bike rentals at noon
   - Feature selection based on exploratory analysis

2. **Feature Selection**:
   - Visualization of relationships between features and bike count
   - Removal of less important features (wind, visibility, functioning day status)

3. **Model Development**:
   - Simple linear regression with temperature only
   - Multiple linear regression with all relevant features
   - Neural network regression models for comparison

4. **Model Evaluation**:
   - R-squared comparison
   - Mean Squared Error (MSE) comparison
   - Visual comparison of predictions against ground truth

## Key Findings

- Temperature shows a significant correlation with bike rental demand
- Multiple regression with several features outperforms simple linear regression
- Neural networks can capture more complex relationships in the data than linear models
- The project demonstrates the practical differences between traditional statistical approaches and machine learning methods

## Usage Examples

Open the Jupyter notebook to see the analysis:

```bash
jupyter notebook linear_regression.ipynb
```

The notebook contains all code with explanations of each step in the modeling process.

## Visualizations

The project includes various visualizations:
- Scatter plots showing the relationship between individual features and bike count
- Fitted regression lines showing predicted relationships
- Learning curves for neural network training
- Comparison plots of predicted vs. actual values

## License

This project uses publicly available data from the UCI Machine Learning Repository. Please cite the original dataset when using this code for academic or research purposes.
