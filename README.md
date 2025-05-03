# 🧪 PCA on Breast Cancer Dataset

This project demonstrates the application of **Principal Component Analysis (PCA)** on the Breast Cancer dataset available in `sklearn.datasets`. PCA is used to reduce the dimensionality of the dataset and visualize the data in lower dimensions while retaining most of the variance.

---

## 📊 Dataset

The dataset is loaded using:

```python
from sklearn.datasets import load_breast_cancer
```

It contains **569 samples** with **30 numerical features** and a binary classification target:
- `target = 0`: malignant
- `target = 1`: benign

---

## 🔍 Steps Performed

1. **Data Loading**
   - Load the Breast Cancer dataset using `load_breast_cancer()`.
   - Convert the data to a Pandas DataFrame for easier analysis.

2. **Data Exploration**
   - Display the shape and summary statistics.
   - Visualize class distribution.

3. **Data Standardization**
   - Standardize the features using `StandardScaler` to ensure all variables contribute equally to the PCA.

4. **PCA Transformation**
   - Apply PCA using `sklearn.decomposition.PCA`.
   - Analyze the explained variance ratio to determine how many components to retain.

5. **Visualization**
   - Plot the data in the first two principal components.
   - Visualize explained variance via a scree plot.

6. **Insights**
   - Examine how well PCA separates the two classes.
   - Observe how much variance is captured by the top components.

---

## 📈 Results

- The first 2 principal components typically capture ~95% of the total variance.
- PCA is able to separate malignant and benign samples fairly well in 2D space.

---

## 🛠️ Requirements

Install dependencies via:

```bash
pip install numpy pandas matplotlib seaborn scikit-learn
```

---

## 🚀 How to Run

```bash
python pca_breast_cancer.py
```

Make sure the script includes the visualizations and printed outputs for analysis.

---

## 📎 References

- [scikit-learn documentation – PCA](https://scikit-learn.org/stable/modules/generated/sklearn.decomposition.PCA.html)
- [Breast Cancer Dataset](https://scikit-learn.org/stable/datasets/toy_dataset.html#breast-cancer-dataset)

