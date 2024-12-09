# California Housing Price Prediction using XGBoost

This project uses the **California Housing dataset** to predict median housing prices in California neighborhoods. The workflow demonstrates skills in data analysis, visualization, feature engineering, and building a regression model using **XGBoost**, one of the most powerful and efficient machine learning algorithms.

---

## Project Overview

The goal of this project is to predict the **median house value** (`MedHouseVal`) in California using features such as population density, median income, and average number of rooms. The project includes:

- **Data Loading & Exploration**: Understanding the dataset and its features.
- **Data Preprocessing**: Handling missing values, feature scaling, and dataset splitting.
- **Model Training**: Using the **XGBoost Regressor** for predictions.
- **Model Evaluation**: Assessing performance using **R-squared** and **Mean Absolute Error (MAE)**.
- **Visualization**: Understanding feature correlations and visualizing predictions against actual prices.

---

## Dataset: California Housing

- **Source**: The California Housing dataset is a built-in dataset from the `sklearn` library.
- **Features**:
  - `MedInc`: Median income in the block group.
  - `HouseAge`: Median age of houses.
  - `AveRooms`: Average number of rooms per household.
  - `AveBedrms`: Average number of bedrooms per household.
  - `Population`: Block group population.
  - `AveOccup`: Average number of occupants per household.
  - `Latitude`: Latitude coordinate of the block group.
  - `Longitude`: Longitude coordinate of the block group.
- **Target**:
  - `MedHouseVal`: Median house value in the block group.

The dataset contains **20,640 rows and 9 columns**, providing a robust foundation for predictive analysis.

---

## Methodology

1. **Exploratory Data Analysis (EDA)**:
   - Generated statistical summaries using `.describe()`.
   - Visualized correlations between features using a **heatmap**.

2. **Feature Selection**:
   - Excluded the target variable (`MedHouseVal`) from predictors.

3. **Data Splitting**:
   - Split the dataset into **80% training** and **20% testing** sets using `train_test_split()`.

4. **Model Training**:
   - Built and trained the **XGBoost Regressor** on the training set.
   - Optimized hyperparameters to improve performance.

5. **Model Evaluation**:
   - Assessed the model using:
     - **R-squared Score**: Measures how well predictions match the actual values.
     - **Mean Absolute Error (MAE)**: Quantifies prediction errors.
   - Visualized the relationship between actual and predicted housing prices using scatter plots.

---

## Key Results

- **Training Set Evaluation**:
  - **R-squared Score**: 0.94 (excellent performance on training data).
  - **Mean Absolute Error (MAE)**: Low prediction error on the training set.

- **Test Set Evaluation**:
  - **R-squared Score**: Achieved high accuracy on unseen data.
  - **Mean Absolute Error (MAE)**: Model generalizes well to the test set.

- **Visualization**:
  - Scatter plot of actual vs. predicted prices shows a strong correlation, indicating reliable predictions.

---

## Skills Demonstrated

- **Machine Learning**: Applied regression techniques using XGBoost.
- **Python Libraries**:
  - **Pandas** for data manipulation.
  - **NumPy** for numerical computations.
  - **Matplotlib** and **Seaborn** for data visualization.
  - **Sklearn** for preprocessing, model evaluation, and dataset management.
- **Data Visualization**: Created insightful plots to communicate findings.
- **Model Evaluation**: Leveraged appropriate metrics for regression problems.

---

## How to Run

1. Clone this repository:
   ```bash
   git clone <repository-url>
   cd <repository-folder>
   ```

2. Install required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Run the script:
   ```bash
   python california_housing_prediction.py
   ```

---

## Future Work

- Perform hyperparameter tuning to further improve model performance.
- Implement additional regression models for comparison (e.g., Random Forest, Linear Regression).
- Deploy the model as a web application using Flask or Streamlit.

---

This project demonstrates practical experience in machine learning and predictive analytics, making it relevant for roles in **data science**, **machine learning**, and **business analytics**. Feel free to explore the code and reach out with any questions or feedback.
