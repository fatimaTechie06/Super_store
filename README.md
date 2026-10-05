# 🛒 Outlet Sales Prediction using KNN Regression

## 📌 Project Overview

This project is a **Machine Learning-based Outlet Sales Prediction System** that predicts outlet sales using the **K-Nearest Neighbors (KNN) Regression** algorithm.

The project includes a **Flask web application** where users can enter product and outlet details and receive a predicted sales value.

---

## 🎯 Objectives

* Predict outlet sales using Machine Learning.
* Apply **KNN Regression** to a real-world sales prediction problem.
* Process categorical and numerical input features.
* Build a user-friendly web interface using Flask.
* Generate real-time sales predictions from user-provided data.

---

## 🤖 Machine Learning Algorithm

### K-Nearest Neighbors (KNN) Regression

KNN Regression predicts the target value by finding the nearest data points to the given input and using their values to estimate the prediction.

**Model Used:** KNN Regression

The trained model is stored as:

```text
knn_regression_model.pkl
```

---

## 📊 Input Features

The application accepts the following information:

### Product Features

* Item Weight
* Item Fat Content
* Item Visibility
* Item MRP
* Item Type

### Outlet Features

* Outlet Size
* Outlet Location Type
* Outlet Establishment Year
* Outlet Identifier
* Outlet Type

---

## ⚙️ Project Workflow

```text
Dataset
   ↓
Data Preprocessing
   ↓
Feature Encoding
   ↓
KNN Regression Model
   ↓
Model Training
   ↓
Model Saving (.pkl)
   ↓
Flask Web Application
   ↓
User Input
   ↓
Sales Prediction
```

---

## 🌐 Web Application

The project uses **Flask** to provide a web interface.

The application contains:

* Home page for entering input data.
* Prediction functionality.
* Real-time sales prediction.
* Automatic preprocessing of categorical features.
* Display of predicted sales.

The Flask application loads the trained KNN model and uses the same feature structure as the training data.

---

## 🔄 Data Preprocessing

Categorical variables are converted into numerical form using **One-Hot Encoding**.

The application processes:

* `Item_Type`
* `Outlet_Identifier`
* `Outlet_Type`

The generated features are aligned with the feature order expected by the trained model before making predictions.

---

## 🗂️ Project Structure

```text
Outlet-Sales-Prediction/
│
├── app(4).py
├── KNN Regression.ipynb
├── KNN_reg_outlet_sales - KNN_reg_outlet_sales.csv
├── knn_regression_model.pkl
├── templates/
│   └── index.html
│
└── README.md
```

---

## 🛠️ Technologies Used

* **Python**
* **Pandas**
* **Scikit-learn**
* **Flask**
* **Jupyter Notebook**
* **Machine Learning**
* **KNN Regression**
* **HTML/CSS**

---

## 🚀 Installation and Setup

### 1. Clone the Repository

```bash
git clone <your-github-repository-url>
```

### 2. Open the Project Folder

```bash
cd Outlet-Sales-Prediction
```

### 3. Install Required Libraries

```bash
pip install flask pandas scikit-learn
```

### 4. Run the Flask Application

```bash
python app(4).py
```

If your file is renamed to `app.py`, use:

```bash
python app.py
```

### 5. Open in Browser

Open the local Flask address shown in the terminal, usually:

```text
http://127.0.0.1:5000/
```

---

## 🔮 Prediction Process

The user enters product and outlet information through the web form.

The application:

1. Receives the user input.
2. Creates a Pandas DataFrame.
3. Encodes categorical features.
4. Matches the training feature structure.
5. Sends the processed data to the KNN model.
6. Generates the predicted sales value.
7. Displays the prediction on the webpage.

---

## 📈 Example Inputs

| Feature                   | Example           |
| ------------------------- | ----------------- |
| Item Weight               | 12.5              |
| Item Fat Content          | Low Fat           |
| Item Visibility           | 0.05              |
| Item MRP                  | 150               |
| Outlet Size               | Medium            |
| Outlet Location Type      | Tier 2            |
| Outlet Establishment Year | 2004              |
| Item Type                 | Dairy             |
| Outlet Identifier         | OUT049            |
| Outlet Type               | Supermarket Type1 |

---

## 💡 Key Features

✅ KNN Regression-based prediction
✅ Flask web application
✅ Real-time sales prediction
✅ Numerical and categorical feature handling
✅ One-Hot Encoding
✅ Pre-trained model using `.pkl` file
✅ Simple and user-friendly interface

---

## 🔮 Future Enhancements

* Add graphical visualization of predicted sales.
* Improve model performance using hyperparameter tuning.
* Compare KNN with Random Forest, Linear Regression and other algorithms.
* Add prediction history.
* Deploy the application online.
* Add an interactive dashboard for sales analysis.

---

## 📚 Dataset

The project uses an **Outlet Sales dataset** containing product-related and outlet-related information.

The dataset file used in the project is:

```text
KNN_reg_outlet_sales - KNN_reg_outlet_sales.csv
```

---

## 👩‍💻 Project Type

**Machine Learning Mini Project**

**Domain:** Sales Prediction / Retail Analytics

**Algorithm:** K-Nearest Neighbors Regression

**Application:** Web-based Sales Prediction System

---

## 📜 License

This project is created for **educational and academic purposes**.
