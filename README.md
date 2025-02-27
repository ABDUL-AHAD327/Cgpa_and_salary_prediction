# CGPA vs Salary Prediction using Linear Regression

## Overview

This project implements a **Linear Regression model** to predict a student's expected salary package (in LPA) based on their CGPA. The dataset is obtained from Kaggle, and the model is trained using **gradient descent** as well as **Scikit-Learn's LinearRegression**.

## Dataset

- **Source:** Kaggle (parvmodi/cgpa-vs-package-in-lpa)
- **Features:**
  - **CGPA** (Continuous Variable)
  - **Salary Package (LPA)** (Target Variable)
- **Size:** 200 samples

## Steps Implemented

1. **Data Loading & Preprocessing:**

   - Load dataset using Pandas
   - Check dataset structure (number of rows, missing values, etc.)
   - Visualize data using scatter plots

2. **Gradient Descent Implementation:**

   - Initialize parameters (theta\_0, theta\_1)
   - Optimize cost function using **Gradient Descent** for 10 iterations
   - Plot cost function per iteration

3. **Train Model using Scikit-Learn:**

   - Use `LinearRegression()` from Scikit-Learn
   - Train model and extract optimized parameters
   - Compare results with manually implemented gradient descent

4. **Visualizing Regression Line:**

   - Plot best-fit line over the scatter plot
   - Compare different methods for optimization

5. **Testing on New CGPA Data:**

   - Predict salaries for user-input CGPA values
   - Ensure input CGPA is within dataset range

## Installation & Usage

### **1. Install Dependencies**

```bash
pip install numpy pandas matplotlib scikit-learn kagglehub
```

### **2. Run the Notebook or Script**

- If using Jupyter Notebook:

```bash
jupyter notebook cgpa_vs_salary.ipynb
```

- If running as a Python script:

```bash
python cgpa_vs_salary.py
```

### **3. Test the Model on New Data**

Modify the following in the script to test custom CGPA values:

```python
new_cgpa = np.array([6.5, 8.2, 9.0]).reshape(-1, 1)
predicted_salaries = model.predict(new_cgpa)
```

## Example Output

```
Predicted Salary for CGPA 6.5: 3.25 LPA
Predicted Salary for CGPA 7.8: 3.85 LPA
Predicted Salary for CGPA 9.2: 4.45 LPA
```

## Future Enhancements

- Use **multiple regression** (add more factors like internships, projects, etc.)
- Implement **polynomial regression** for better accuracy
- Deploy as a **web app using Flask or Streamlit**

## Author

Your Name -ABDUL AHAD MALIK

License

This project is open-source under the MIT License.

