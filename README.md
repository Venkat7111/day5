# 🌳 Decision Tree vs Random Forest Classifier (Scikit-learn + Graphviz)

This mini project demonstrates classification using Decision Trees and Random Forests with model visualization and evaluation.

---

## 🎯 Tasks Covered

1. ✅ Train a **Decision Tree Classifier** and visualize the tree using **Graphviz**.
2. ✅ Analyze **overfitting** by controlling `max_depth` and plotting accuracy.
3. ✅ Train a **Random Forest Classifier** and compare its accuracy with the Decision Tree.
4. ✅ Interpret **feature importances** using Random Forest.
5. ✅ Evaluate both models using **cross-validation** with `cross_val_score()`.

---

## 🛠️ Technologies Used

- Python
- Scikit-learn
- Graphviz
- Pandas
- Matplotlib
- Google Colab (for development)

---

## 📁 Dataset

**Iris Dataset** (built-in from Scikit-learn):
- **Features**: 
  - Sepal Length
  - Sepal Width
  - Petal Length
  - Petal Width
- **Targets**:
  - Setosa
  - Versicolor
  - Virginica

---

## ✅ Steps Performed

### 1. Decision Tree Classifier
- Loaded Iris dataset.
- Trained a `DecisionTreeClassifier`.
- Visualized tree with `export_graphviz()` and `graphviz.Source()`.

### 2. Overfitting Control
- Trained multiple Decision Trees with varying `max_depth`.
- Plotted training vs testing accuracy.

### 3. Random Forest Classifier
- Trained `RandomForestClassifier` with 100 estimators.
- Compared accuracy with the Decision Tree on test data.

### 4. Feature Importance
- Extracted `.feature_importances_` from Random Forest.
- Visualized with a bar chart using Matplotlib.

### 5. Cross-Validation
- Used `cross_val_score()` with `cv=5`.
- Evaluated both classifiers on mean cross-validation accuracy.

---

## 📊 Sample Results

| Model           | Test Accuracy | CV Accuracy |
|----------------|---------------|-------------|
| Decision Tree  | ~0.89         | ~0.95       |
| Random Forest  | ~0.96         | ~0.97       |

> 🔍 *Random Forest tends to perform better due to ensemble averaging.*

---

## ▶️ How to Run in Google Colab

1. Open the `.ipynb` notebook or paste the code blocks.
2. Run the following to install dependencies:

```python
!pip install graphviz
!apt-get install -y graphviz
