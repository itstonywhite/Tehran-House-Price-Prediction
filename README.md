# Tehran House Price Prediction

## Project Overview

This project applies Machine Learning techniques to predict house prices in Tehran based on a dataset of approximately 4,000 real estate listings. Using **Multiple Linear Regression**, the model estimates the price of a property given its specific features.

## Dataset

The dataset (`housePrice.csv`) contains real-world housing data in Tehran with the following features:

- **Area**: Size of the property in square meters.
- **Room**: Number of bedrooms.
- **Parking**: Boolean indicator for parking availability.
- **Warehouse**: Boolean indicator for storage/warehouse availability.
- **Elevator**: Boolean indicator for elevator availability.
- **Address**: The neighborhood/district in Tehran.
- **Price**: Target variable (in Toman).
- **Price(USD)**: Target variable in USD (Excluded during training to prevent data leakage).

## Data Processing & Methodology

1. **Data Cleaning**: Handled missing categorical data (empty addresses) and resolved formatting issues with numeric columns. Extreme outliers in the 'Area' column were removed to ensure model robustness.
2. **Feature Engineering**: Applied **One-Hot Encoding** to handle the categorical `Address` variable and boolean features.
3. **Scaling**: Used `StandardScaler` to normalize data distributions prior to training.
4. **Modeling**: Built and trained a Multiple Linear Regression model using `scikit-learn`.

## Technologies Used

- **Python 3**
- **Pandas & NumPy** (Data Manipulation)
- **Scikit-learn** (Machine Learning Pipeline & Evaluation)
- **Matplotlib & Seaborn** (Data Visualization)

## Results

The model's performance was evaluated using standard regression metrics.

- **R-squared (R2 Score)**: Demonstrates the variance explained by the model.
- **Mean Absolute Error (MAE)**: Shows the average absolute difference between actual and predicted prices.

* **Mean Squared Error (MSE)**: Penalizes larger errors by squaring the differences before averaging, providing insight into the model's variance.

## 📦 Installation Guide

Follow these steps to set up the project on your local machine:

1. Clone the repository:

```bash
git clone https://github.com/itstonywhite/tehran-house-price-prediction.git
```

2. Make sure you have the required libraries installed:

```bash
pip install pandas numpy scikit-learn matplotlib seaborn joblib
```

3. Open `House Price Prediction.ipynb` using Jupyter Notebook, Google Colab or VS Code and run all cells.

---

_This is my very first machine learning project :)_

\- [Tony White ✍️](https://github.com/itstonywhite)
