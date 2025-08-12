# Assignment 1 – Polynomial Regression (Cars Dataset)

This project explores a dataset of cars and uses various data analysis and regression techniques to understand and model the relationship between features such as horsepower and miles-per-gallon (MPG).

---

## 📌 Objective

- Explore the relationship between car features and fuel economy.
- Handle missing data through appropriate imputation.
- Use both linear and polynomial regression techniques.
- Visualize data distributions and trends.
- Implement gradient descent for linear regression.

---

## 📂 Dataset

- **File**: `cars.csv`
- **Features**:
  - `mpg`: Miles per gallon (target)
  - `cylinders`, `displacement`, `horsepower`, `weight`, `acceleration`, `model_year`, `origin`

---

## 🔢 Steps & Analysis

### 1. **Read Dataset**
- Loaded `cars.csv` using `pandas`

### 2. **Handle Missing Values**
- `horsepower`: 6 missing values → filled with **median**
- `origin`: 2 missing values → filled with **mode**

### 3. **Fuel Economy by Country**
- Boxplot showing MPG across different `origin` values (USA, Europe, Asia)
- Median MPG:
  - Asia: 31.55
  - Europe: 26.50
  - USA: 18.55

### 4. **Feature Distributions**
- Histograms + KDE for:
  - `mpg`
  - `acceleration`
  - `horsepower`

### 5. **Skewness Measurement**
Quantitative measure to support histogram visuals:
| Feature       | Skewness |
|---------------|----------|
| mpg           | 0.46     |
| acceleration  | 0.28     |
| horsepower    | 1.11     |

### 6. **Scatter Plot: Horsepower vs MPG**
- Strong **negative correlation**: **-0.77**

---

## 📈 Regression Models

### 🔹 Linear Regression (Closed Form)
- Target: Predict `mpg` from `horsepower`
- Equation:  
  **mpg = 40.01 − 0.16 × horsepower**

### 🔹 Quadratic Regression
- Equation:  
  **mpg = 56.78 − 0.46 × horsepower + 0.00 × horsepower²**

### 🔹 Linear Regression (Gradient Descent)
- Implemented from scratch
- Learning rate: 0.0001  
- Converged after **716,295 iterations**
- Final model:  
  **mpg = 40.00 − 0.16 × horsepower**

---

## 🛠️ Technologies

- Python 3
- Pandas, NumPy
- Matplotlib, Seaborn
- Scipy (for skewness)
- Google Colab

---

## 📊 Key Insights

- `horsepower` is a strong predictor of `mpg`
- USA cars tend to have lower fuel economy
- Feature skewness highlights the need for preprocessing
- Gradient descent and closed-form produce consistent results





