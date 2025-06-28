# 🩺 Diabetes Prediction System using Machine Learning

This project predicts whether a person is diabetic or not using a Machine Learning model trained on the **PIMA Indian Diabetes Dataset**. The system uses medical parameters like glucose levels, BMI, age, etc., to classify patients.

✅ Built using Python, Scikit-learn, Pandas, NumPy, and Google Colab.  
✅ Ideal for beginners in Machine Learning and healthcare-related ML projects.

---

## 📂 Table of Contents

- [Project Overview](#project-overview)
- [Dataset Details](#dataset-details)
- [Technologies Used](#technologies-used)
- [Model and Workflow](#model-and-workflow)
- [How to Run](#how-to-run)
- [Prediction Example](#prediction-example)
- [Output Screenshot](#output-screenshot)
- [Project Links](#project-links)
- [Future Improvements](#future-improvements)

---

## 📊 Project Overview

The project uses a **Support Vector Machine (SVM)** classifier to predict diabetes risk based on patient attributes. It applies preprocessing techniques like feature scaling to improve model performance.

---

## 📑 Dataset Details

The dataset used is the **PIMA Indian Diabetes Dataset**, available on:

[Kaggle: PIMA Indian Diabetes Database](https://www.kaggle.com/datasets/uciml/pima-indians-diabetes-database)

It contains 768 rows and 8 medical features:

- Pregnancies
- Glucose
- Blood Pressure
- Skin Thickness
- Insulin
- BMI
- Diabetes Pedigree Function
- Age

Target Variable:
- `1` - Diabetic  
- `0` - Not Diabetic  

---

## ⚙️ Technologies Used

- Python 3.x
- NumPy
- Pandas
- Scikit-learn
- Google Colab / Jupyter Notebook

---

## 🧠 Model and Workflow

1. Load dataset with Pandas
2. Preprocess data with `StandardScaler`
3. Train-Test split (80-20)
4. Train SVM Classifier (`linear` kernel)
5. Evaluate using Accuracy Score
6. Make predictions for new patient data

---

## 🚀 How to Run

✅ **Option 1:** [Open in Google Colab](https://colab.research.google.com/github/pratik-pritam-rout/Diabetes-Prediction-ML/blob/main/Diabetes_Prediction.ipynb)

✅ **Option 2:** Clone the repository:

```bash
git clone https://github.com/pratik-pritam-rout/Diabetes-Prediction-ML.git
cd Diabetes-Prediction-ML
Open Diabetes_Prediction.ipynb with Jupyter or Colab, run all cells in order.

🔮 Prediction Example
python
Copy
Edit
input_data = (1, 85, 66, 29, 0, 26.6, 0.351, 31)

columns = ['Pregnancies', 'Glucose', 'BloodPressure', 'SkinThickness',
           'Insulin', 'BMI', 'DiabetesPedigreeFunction', 'Age']

input_df = pd.DataFrame([input_data], columns=columns)
input_data_scaled = scaler.transform(input_df)
prediction = classifier.predict(input_data_scaled)

if prediction[0] == 0:
    print("The person is not diabetic")
else:
    print("The person is diabetic")
📸 Output Screenshot
Example console output:
The person is not diabetic

Accuracy Score: 77%
