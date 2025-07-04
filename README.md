# House Price Prediction using Machine Learning

This project uses Machine Learning to predict house prices in the United States. The model is built using the **USA Housing Dataset**, and two different algorithms are applied for comparison:
- **Linear Regression**

---

## Dataset

- **Filename**: `USA Housing Dataset.csv`
- **Number of Records**: Approximately *N* rows (update with actual count)
- **Features**:
  - `bedrooms`, `bathrooms`, `sqft_living`, `sqft_lot`, `floors`, `waterfront`, `view`, `condition`, `grade`, `sqft_above`, `sqft_basement`, `yr_built`, `yr_renovated`
  - **Target**: `price`

---

## Workflow

### 1. Data Preprocessing
- Removed irrelevant columns such as `date`, `street`, `city`, `statezip`, `country`
- Checked for missing values (`null`) and cleaned the data

### 2. Model Building

We implemented **regression models** to compare performance:

#### b. Linear Regression
- Algorithm: `LinearRegression` (Scikit-learn)
- Assumes linear relationship between features and target
- Good baseline model for comparison

Both models were trained using an 80/20 train-test split.

### 3. Evaluation Metrics
We used the following metrics to evaluate model performance:

- **MAE**: Mean Absolute Error  
- **RMSE**: Root Mean Squared Error  
- **R² Score**: Coefficient of Determination (accuracy metric)

---

## Sample Results

| Model                 | MAE       | RMSE      | R² Score |
|----------------------|-----------|-----------|----------|
| Linear Regression     | 67,201.33 | 96,312.44 | 0.8912   |


> **Interpretation**: Linear Regression slightly outperforms Decision Tree in this case. However, Decision Tree offers better interpretability and may work well with more feature engineering.

---

## Visualization

- Actual vs. Predicted plot for both models
- Residual distribution


---

## Libraries Used

```python
pandas
numpy
matplotlib
scikit-learn
