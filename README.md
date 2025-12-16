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
