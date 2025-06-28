# 🩺 Diabetes Prediction System using Machine Learning

This project uses a Support Vector Machine (SVM) classifier to predict whether a person is likely to have diabetes based on medical attributes. It is built using Python and trained on the **PIMA Indian Diabetes Dataset**.

---

## 📊 Dataset

The dataset used is publicly available from the [UCI Machine Learning Repository](https://www.kaggle.com/datasets/uciml/pima-indians-diabetes-database), which contains medical data of female patients of Pima Indian heritage.

### Features include:
- Pregnancies
- Glucose
- Blood Pressure
- Skin Thickness
- Insulin
- BMI
- Diabetes Pedigree Function
- Age

---

## 🧠 Technologies Used

- Python 🐍
- NumPy
- Pandas
- Scikit-learn
- Google Colab

---

## 🚀 How to Run the Project

1. Open the notebook in Google Colab or Jupyter Notebook.
2. Run all the cells in order.
3. The model will be trained using an 80-20 train-test split.
4. Enter a sample input to check predictions.

---

## 🧪 Model Used

- **Algorithm**: Support Vector Machine (SVM) with linear kernel
- **Preprocessing**: Feature scaling using `StandardScaler`
- **Evaluation**: Accuracy score on the test set

---

## 📈 Sample Input

```python
input_data = (1, 85, 66, 29, 0, 26.6, 0.351, 31)
