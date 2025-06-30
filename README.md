# 🏠 House Price Prediction using Machine Learning

This project uses Machine Learning to predict house prices in the United States. The model is built using the **USA Housing Dataset** and implemented with the **Decision Tree Regressor** from the Scikit-learn library in Python.

---

## 📁 Dataset

- **Filename**: `USA Housing Dataset.csv`
- **Number of Records**: Approximately *N* rows (update with actual count)
- **Features**:
  - `bedrooms`, `bathrooms`, `sqft_living`, `sqft_lot`, `floors`, `waterfront`, `view`, `condition`, `grade`, `sqft_above`, `sqft_basement`, `yr_built`, `yr_renovated`
  - **Target**: `price`

---

## ⚙️ Workflow

### 1. Data Preprocessing
- Removed irrelevant columns such as `date`, `street`, `city`, `statezip`, `country`
- Checked for missing values (`null`) and cleaned the data

### 2. Model Building

We implemented **two regression models** to compare performance:

#### a. Decision Tree Regressor
- Algorithm: `DecisionTreeRegressor` (Scikit-learn)
- Simple and interpretable model
- Tunable parameters: `max_depth`, `min_samples_split`, etc.

#### b. Linear Regression
- Algorithm: `LinearRegression` (Scikit-learn)
- Assumes linear relationship between features and target
- Good baseline model for comparison

Both models were trained using an 80/20 train-test split.

### 3. Evaluation Metrics
- **MAE**: Mean Absolute Error
- **RMSE**: Root Mean Squared Error
- **R² Score**: Coefficient of Determination (accuracy metric)

---

## 📊 Sample Results

```text
Mean Absolute Error (MAE): 72,583.45
Root Mean Squared Error (RMSE): 103,421.97
R² Score: 0.8641
