 Assignment #2 – Polynomial & Logistic Regression

This project demonstrates the implementation of **Polynomial Regression**, **Ridge Regression**, and **Logistic Regression (Linear & Quadratic Decision Boundaries)** using Python and scikit-learn.

> ✅ **Note:** This notebook was originally developed in Google Colab.  
> 📌 Make sure your Google Drive contains the following 3 CSV files:
- `data_reg.csv`
- `train_cls.csv`
- `test_cls.csv`

---

## 📂 Project Structure

- **Data Preparation**
  - Mount Google Drive
  - Read dataset `data_reg.csv`
  - Split into training (120), validation (40), and testing (40)

- **3D Data Visualization**
  - Scatter plot showing the 3 sets in 3D using x1, x2, and y.

- **Polynomial Regression**
  - Trained using polynomial degrees from 1 to 10.
  - Validation MSE plotted to find the optimal degree.
  - Degree 2 achieved the best performance (MSE ≈ 0.1799).

- **Ridge Regression**
  - Applied on degree 8 polynomial.
  - Tested different regularization parameters: `[0.001, 0.005, 0.01, 0.1, 10]`
  - Best performance at `alpha = 0.01` with MSE ≈ 0.2099.

- **Logistic Regression**
  - **Linear Decision Boundary**:
    - Applied on `train_cls.csv` and `test_cls.csv`
    - Accuracy, precision, recall, and F1-score computed.
    - Decision boundary plotted for both train and test sets.
  
  - **Quadratic Decision Boundary**:
    - Polynomial features (degree 2) used.
    - Model retrained and evaluated similarly.
    - Decision boundary shows improved separation of classes.

- **Model Evaluation**
  - Discussion on overfitting vs. underfitting between linear and quadratic models.

---

## 🔧 Technologies Used

- Python
- Google Colab
- pandas, numpy, matplotlib
- scikit-learn

---

## 🚀 How to Run

1. Open the notebook in [Google Colab](https://colab.research.google.com/)
2. Make sure your Google Drive is mounted and includes the required files.
3. Run all cells step-by-step to:
   - Load and visualize the data
   - Train and evaluate models
   - Plot results

---


## 🧠 Notes

- Polynomial regression of high degree may lead to overfitting.
- Regularization helps control model complexity.
- Quadratic logistic regression improved performance compared to the linear version.

