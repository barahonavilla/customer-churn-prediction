## Project Overview

This project focuses on predicting customer churn using machine learning techniques. The goal is to identify customers who are likely to stop using a service, allowing businesses to take preventive actions.

The project includes data preprocessing, feature engineering, model training, and evaluation.

---

## Technologies Used

- PySpark (data processing)
- Pandas & NumPy
- Scikit-learn
- Jupyter Notebook

---

## Data Processing

The dataset was preprocessed using PySpark, including:

- Handling missing values
- Feature scaling using Min-Max normalization
- Encoding categorical variables manually
- Creation of new features such as:
  - `days_since_last_purchase`

---

## Models Evaluated

Three models were trained and compared:

1. Logistic Regression (baseline)
2. Logistic Regression (class balanced)
3. Random Forest

---

## 📊 Results

| Model                         | Accuracy | Recall (Churn) |
|--------------------------------|----------|----------------|
| Logistic Regression            | ~0.80     | 0.00 |
| Logistic Regression (balanced) | ~0.52     | ~0.46 |
| Random Forest                  | ~0.77     | ~0.06 |

---

## Key Findings

- Accuracy is not a reliable metric for imbalanced datasets
- The baseline model failed to detect churn cases
- Class balancing significantly improved recall
- Random Forest achieved good accuracy but poor churn detection

---

## Business Insight

From a business perspective, identifying churn customers is more important than achieving high accuracy.

The balanced Logistic Regression model provides a better trade-off by improving recall for churn prediction.

---

## Future Improvements

- Adjust classification threshold
- Apply resampling techniques
- Use more advanced models (e.g., Gradient Boosting)
- Hyperparameter tuning

---

## Conclusion

This project highlights the importance of handling class imbalance and selecting appropriate evaluation metrics in machine learning problems.
