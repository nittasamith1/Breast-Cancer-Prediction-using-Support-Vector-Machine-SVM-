
# Breast Cancer Prediction using Support Vector Machine (SVM) 🚀

## 📌 Project Overview

This project predicts whether a breast tumor is **Benign (B)** or **Malignant (M)** using the **Support Vector Machine (SVM)** Machine Learning algorithm.

The project includes:

* Data preprocessing
* Feature scaling
* Data visualization
* SVM model training
* Accuracy evaluation
* Confusion matrix visualization
* Decision boundary plotting

---

# 📂 Dataset

Dataset used:

* Breast Cancer Wisconsin Dataset

Target Column:

* `diagnosis`

  * `B` → Benign
  * `M` → Malignant

---

# 🛠 Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn

---

# 📦 Required Libraries

Install dependencies using:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
````

---

# 🚀 Project Workflow

## 1. Import Libraries

```python
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns
```

---

## 2. Load Dataset

```python
df = pd.read_csv("breast-cancer.csv")
```

---

## 3. Data Preprocessing

* Remove unnecessary columns
* Handle target labels
* Feature selection
* Feature scaling

---

## 4. Feature Scaling

```python
from sklearn.preprocessing import StandardScaler
```

Feature scaling is important because SVM depends on distance calculations.

---

## 5. Train-Test Split

```python
from sklearn.model_selection import train_test_split
```

Dataset is divided into:

* Training Data
* Testing Data

---

## 6. Train SVM Model

```python
from sklearn.svm import SVC

model = SVC(
    kernel='rbf',
    C=1,
    gamma='scale'
)
```

---

# ⭐ Important SVM Parameters

| Parameter | Description                             |
| --------- | --------------------------------------- |
| `C`       | Controls margin vs classification error |
| `kernel`  | Type of decision boundary               |
| `gamma`   | Controls boundary complexity            |

---

# 📊 Data Visualization

Scatter plots are used to visualize:

* Benign tumors
* Malignant tumors
* Feature relationships

Example:

```python
sns.scatterplot(
    x='radius_mean',
    y='texture_mean',
    hue='diagnosis',
    data=df
)
```

---

# 📈 Model Evaluation

The project evaluates:

* Accuracy Score
* Confusion Matrix
* Classification Report

---

# 📉 Confusion Matrix

```python
from sklearn.metrics import confusion_matrix
```

Heatmap visualization is used for better understanding.

---

# 🧠 Important Features Used

* radius_mean
* texture_mean
* perimeter_mean
* area_mean
* compactness_mean
* concavity_mean
* concave points_mean
* radius_worst
* perimeter_worst
* area_worst

---

# 📌 Why Use SVM?

Support Vector Machine is effective for:

* Binary classification
* High-dimensional datasets
* Medical prediction systems

Advantages:

* High accuracy
* Effective decision boundaries
* Works well with smaller datasets

---

# 📊 SVM Decision Boundary

The project also visualizes:

* Decision boundary
* Support vectors
* Training data separation

This helps understand how SVM classifies tumors.

---

# 📷 Output

The model predicts:

* Benign Tumor
* Malignant Tumor

with high classification accuracy.

---

# 🎯 Future Improvements

* Hyperparameter tuning
* Streamlit web app deployment
* Cross-validation
* Feature importance analysis
* Real-time prediction interface

---

# 📚 Machine Learning Concepts Used

* Supervised Learning
* Classification
* Feature Scaling
* Kernel Trick
* Margin Maximization
* Support Vectors

---

# ⭐ Interview Questions Covered

* What is SVM?
* What are support vectors?
* Why feature scaling is important?
* Difference between linear and RBF kernel?
* What is C parameter?
* What is gamma?
* Why use SVM for classification?

---

# 🏁 Conclusion

This project demonstrates how Support Vector Machine (SVM) can accurately classify breast cancer tumors using medical diagnostic features. It combines preprocessing, visualization, model training, and evaluation into a complete machine learning workflow.

