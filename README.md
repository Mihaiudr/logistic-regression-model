# Bank Marketing – Logistic Regression Analysis

This project implements a **Logistic Regression** model to predict whether a client will subscribe to a bank term deposit based on financial and marketing campaign data.


## Dataset Overview

- **Filename:** `Bank_data.csv` 

| Column Name     | Type    | Description |
|-----------------|---------|-------------|
| `interest_rate` | float   | Interest rate associated with the customer |
| `credit`        | float   | Customer credit score or credit-related metric |
| `march`         | float   | Contact indicator during March |
| `may`           | float   | Contact indicator during May |
| `previous`      | float   | Number of previous contacts made before this campaign |
| `duration`      | float   | Duration of the last contact in seconds |
| `y`             | object  | Target variable: `"yes"` if the customer subscribed, `"no"` otherwise |


##  Objective

The goal is to build a **binary classification model** using Logistic Regression to predict the probability of a client subscribing to a term deposit (`y`).


## Project Steps

1. **Data Loading & Cleaning**
   - Loaded data from `Bank_data.csv`
   - Checked for missing values and data consistency

2. **Exploratory Data Analysis (EDA)**
   - Examined variable distributions and correlations
   

3. **Feature Engineering**
   - Converted categorical variable `y` into numeric (0 = no, 1 = yes)
   - Scaled numeric features for model stability

4. **Model Building**
   - Implemented **Logistic Regression** using `statsmodels` and `sklearn`
   - Trained and validated the model on the dataset

5. **Model Evaluation**
   - Evaluated using:
     - Accuracy
     - Confusion Matrix
   - Interpreted model coefficients to understand feature impact on prediction


## Results

- Logistic Regression achieved strong classification accuracy on the dataset.
- Key influential variables included:
  - **interest_rate**
  - **duration**
  - **previous**

---

## Conclusion

- Logistic Regression effectively modeled the likelihood of client subscription.  
- Longer call durations and lower interest rates were associated with a higher chance of subscription.  
- The model serves as a reliable baseline for future comparisons with more complex algorithms (e.g., Random Forest, XGBoost).


