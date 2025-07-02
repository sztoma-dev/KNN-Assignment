# Custom K-Nearest Neighbors (KNN) Classifier and Regressor

This repository contains **custom from-scratch implementations of the K-Nearest Neighbors (KNN) algorithm** for:

* **Classification** using the **Iris dataset**.
* **Regression** using the **Diabetes dataset**.

**No built-in KNN functions (like from `sklearn`) are used.** All KNN logic (distance calculation, neighbor selection, majority voting, averaging for regression) is implemented manually, following strict academic guidelines.

---

## 📚 Problem Statement

You will:

✅ Prepare and load datasets.
✅ Implement **KNN from scratch (no sklearn, no pandas for algorithm)**.
✅ Tune the parameter `k` and compare validation accuracy (classification) or validation error (regression).
✅ Evaluate the best model on the test set.
✅ Report all results clearly.

---

## 🗂️ Datasets

### Iris Dataset (Classification)

* **Instances:** 150 (50 samples/class)
* **Features:** Sepal length, Sepal width, Petal length, Petal width
* **Classes:** Iris-setosa, Iris-versicolor, Iris-virginica
* [Kaggle Iris Dataset](https://www.kaggle.com/datasets/arshid/iris-flower-dataset)

### Diabetes Dataset (Regression)

* **Instances:** 768
* **Features:** 8 numeric predictive attributes
* **Target:** Disease progression measure
* [Kaggle Diabetes Dataset](https://www.kaggle.com/datasets/akshaydattatraykhare/diabetes-dataset)

---

## 🛠️ Features

* **Manual CSV loading** using Python `csv` module.
* **Random 70-15-15 split** into **Train, Validation, Test** sets using:

  * `0.0 <= R <= 0.7` → Train
  * `0.7 < R <= 0.85` → Validation
  * `0.85 < R <= 1.0` → Test
* **Custom Euclidean distance computation**.
* **Custom neighbor selection and voting (classification)**.
* **Custom neighbor selection and averaging (regression)**.
* **Tuning and comparison for `k = 1, 3, 5, 10, 15`.**
* **Report best k based on validation and evaluate on the test set.**
* **Fully commented, clean, and academic submission ready.**

---

## 🚀 How to Run

1️⃣ Clone the repository:

```bash
git clone https://github.com/yourusername/custom-knn-lab.git
cd custom-knn-lab
```

2️⃣ Place the **Iris.csv** and **Diabetes.csv** in the same directory.

3️⃣ Run KNN Classification:

```bash
python knn_classification.py
```

4️⃣ Run KNN Regression:

```bash
python knn_regression.py
```

---

## 📊 Expected Output

* Prints **validation accuracy for each k** in classification.
* Prints **validation error (MSE) for each k** in regression.
* Shows **test accuracy/error using best k** selected from validation results.

---

## 📝 Marks Distribution (As per lab)

| Task                            | Marks  |
| ------------------------------- | ------ |
| Dataset loading                 | 4      |
| Train/Validation/Test split     | 5      |
| KNN algorithm implementation    | 10     |
| K tuning + validation table     | 3      |
| Best k test accuracy evaluation | 3      |
| **Total**                       | **25** |

---

## ⚠️ Restrictions

✅ No `sklearn`, `scikit-learn`, or `pandas` for the algorithm.
✅ Can only use these libraries for **loading raw CSV if needed**.
✅ All KNN logic must be **implemented manually**.

---

## ✍️ License

This project is for academic learning and practice only. Do not copy for direct submission without understanding.
