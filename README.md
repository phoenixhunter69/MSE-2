# Vegetable Type Classification Using Random Forest

This project uses a **Random Forest Classifier** to predict the type of vegetable based on its nutritional content, including Vitamin A, Vitamin C, and Fiber. The model is trained and evaluated using Python libraries such as pandas, scikit-learn, and seaborn.

---

## 📂 Dataset

The dataset (`vegetables.csv`) includes:
- Nutritional features: `vitamin_a`, `vitamin_c`, `fiber`
- Target feature: `type` (vegetable class/category)

---

## ⚙️ Data Preprocessing

1. **Missing Value Handling**: Numerical columns are filled with their mean values.
2. **Categorical Encoding**: One-hot encoding is used for categorical variables (if any).
3. **Feature Scaling**: StandardScaler is applied to normalize numerical values.
4. **Data Splitting**: The dataset is split into 80% training and 20% testing.

---

## 🧠 Model Building

- A **Random Forest Classifier** is used for training.
- **GridSearchCV** is applied for hyperparameter tuning (`n_estimators`, `max_depth`, `min_samples_split`).
- The best model is selected based on cross-validation accuracy.

---

## 🧪 Evaluation Metrics

- **Accuracy**: Overall correctness of predictions.
- **Precision & Recall**: Performance per class.
- **F1 Score**: Balance between precision and recall.
- **Confusion Matrix**: Visualized using Seaborn for error inspection.

---

## 🔍 Results and Analysis

- The model showed strong performance on the test set.
- Confusion matrix revealed balanced predictions.
- Precision and recall metrics confirmed good detection ability for each vegetable type.

---

## ✅ Conclusion

The Random Forest model effectively classifies vegetable types based on nutritional data. The preprocessing steps and hyperparameter tuning ensured improved accuracy and generalization.

---

## 🧾 References

- [Scikit-learn Documentation](https://scikit-learn.org/stable/documentation.html)
- [Pandas Documentation](https://pandas.pydata.org/docs/)
- [Seaborn Visualization Library](https://seaborn.pydata.org/)
- Research articles on classification and predictive modeling in agriculture

---

## ▶️ Example Usage

```python
classify_vegetable(70.0, 35.0, 8.0)
classify_vegetable(15.0, 80.0, 2.0)
