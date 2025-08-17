# Decision Tree Regression on Position Salary Dataset

## 🎯 Problem Statement and Goal of Project

This project demonstrates the use of a **Decision Tree Regressor** to model and predict salaries based on job position levels. The objective is to explore how **non-linear regression** using decision trees can capture complex patterns in small datasets and make predictions that adapt to data granularity.

---

## 🛠 Solution Approach

The workflow follows a clean regression pipeline:

1. **Data Loading**:

   * Read data from `Position_Salaries.csv`.
2. **Preprocessing**:

   * Extract features and labels (`Level` and `Salary`).
3. **Model Training**:

   * Train a `DecisionTreeRegressor` using all available data (no split for training/testing in the final model).
4. **Prediction**:

   * Predict salary for an intermediate level, e.g., `6.5`.
5. **Visualization**:

   * Plot the fitted decision tree regression curve using a **high-resolution grid** for a clear stepwise structure.

---

## 🧰 Technologies & Libraries

* Python 3
* `pandas`, `numpy` – data processing
* `scikit-learn` – model training and prediction
* `matplotlib`, `seaborn` – visualization

---

## 📁 Dataset Description

* **File:** `Position_Salaries.csv`
* **Features**:

  * `Level`: Position level (1 to 10)
* **Target**:

  * `Salary`: Corresponding salary
* **Goal**:

  * Predict salary for a given position level using decision tree regression.

> Note: This is a small synthetic dataset designed for learning purposes.

---

## ⚙️ Installation & Execution Guide

1. Clone or download this repository.
2. Ensure `Position_Salaries.csv` is in the same directory.
3. Install dependencies:

   ```bash
   pip install numpy pandas matplotlib seaborn scikit-learn
   ```
4. Run the notebook:

   ```bash
   jupyter notebook "Decision Tree (Regression).ipynb"
   ```

---

## 📊 Key Results / Performance

* Model trained on entire dataset for maximum granularity.
* Predicted salary for `level=6.5` using `regressor.predict([[6.5]])`.
* Clear **stepwise prediction pattern** due to decision tree nature.
* Final visualization reveals how decision trees create constant-value segments.

---

## 📸 Sample Outputs

* 🔵 Decision Tree Regression curve
* 🔴 Actual data scatter plot (Position vs Salary)
* ✅ Sample prediction printed for input `6.5`

---

## 📚 Additional Learnings / Reflections

* Demonstrated how **decision trees behave differently in regression** compared to classification.
* Visualized how **splitting thresholds create constant-valued segments**.
* Reinforced the concept of **non-continuous regression** and the importance of model selection based on data behavior.

---

## 👤 Author

## mehran Asgari

**Email:** [imehranasgari@gmail.com](mailto:imehranasgari@gmail.com)
**GitHub:** [https://github.com/imehranasgari](https://github.com/imehranasgari)

---

## 📄 License

This project is licensed under the Apache 2.0 License – see the `LICENSE` file for details.

---

> 💡 *Some interactive outputs (e.g., plots, widgets) may not display correctly on GitHub. If so, please view this notebook via [nbviewer.org](https://nbviewer.org) for full rendering.*

---