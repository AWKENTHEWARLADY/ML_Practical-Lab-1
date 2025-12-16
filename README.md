# CISM-623-Practical-Lab-1
Machine Learning 2025 Practical 


# 🌍 World Population Prediction

## **Project Overview**
This project develops a **Linear Regression model** to predict the population of a specific country using historical population data from **1960 to 2017**. The goal is to provide accurate population estimates for any given year based on historical trends.

The project demonstrates:
- Data extraction and preprocessing
- Train-test splitting
- Model training and evaluation
- Performance measurement using **Mean Squared Error (MSE)**

---

## **Dataset**
The dataset contains world population data for all countries from 1960 to 2017.

**Columns:**
- `Country Name`
- Yearly population columns (`1960, 1961, ..., 2017`)

---

## **Project Workflow**

### **1️⃣ Extract Population Data**
Function: `year_population(country_name)`  
- Input: Country name (`str`)  
- Output: DataFrame with `Year` and `Population`  

```python
data = year_population('Aruba')

2️⃣ Split Data

Function: data_split(df)

Divides data into features (X) and target (y)

Splits into training and testing sets:

test_size = 0.2

random_state = 42

(X_train, y_train), (X_test, y_test) = data_split(data)

3️⃣ Train Linear Regression Model

Function: train_linear_model(X_train, y_train)

Fits a Linear Regression model on the training data

model = train_linear_model(X_train, y_train)

4️⃣ Evaluate Model

Function: evaluate_model(model, X_test, y_test)

Uses Mean Squared Error (MSE) to measure performance

mse = evaluate_model(model, X_test, y_test)
print("Mean Squared Error:", mse)

Installation

Clone the repository and install required dependencies:

git clone <repository-url>
cd world-population-prediction
pip install pandas scikit-learn

Future Improvements

Implement more advanced regression models (Polynomial Regression, Random Forest, etc.)

Provide confidence intervals for predictions

Visualize population trends with plots
