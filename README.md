# 🧠 Customer Churn Prediction App

![Streamlit](https://img.shields.io/badge/Built%20with-Streamlit-FF4B4B?logo=streamlit&logoColor=white)
![TensorFlow](https://img.shields.io/badge/Model-TensorFlow-orange?logo=tensorflow)
![License](https://img.shields.io/badge/License-MIT-blue.svg)
![Status](https://img.shields.io/badge/Status-Deployed-brightgreen)

---

## 📘 Overview
This project is an **AI-powered Customer Churn Prediction System** built with **TensorFlow** and **Streamlit**.  
It predicts whether a bank customer is likely to leave (churn) based on demographic, credit, and activity-related data.

Users can interactively input details such as **Age, Balance, Credit Score, Salary, and more**, and get:
- ✅ Churn Probability
- ✅ Clear Prediction Result (Likely / Not Likely to Churn)

---

## ⚙️ Tech Stack
- **Frontend:** Streamlit  
- **Backend / Model:** TensorFlow (Keras ANN)  
- **Data Handling:** Pandas, NumPy  
- **Preprocessing:** Scikit-learn (Encoders & Scaler)  
- **Deployment:** Streamlit Cloud / Local System  

---

## 📂 Project Structure
📦 customer-churn-prediction
│
├── app.py # Streamlit main app
├── model.h5 # Trained ANN model
├── scaler.pkl # StandardScaler
├── label_encoder_gender.pkl # LabelEncoder for Gender
├── onehot_encoder_geo.pkl # OneHotEncoder for Geography
├── requirements.txt # Dependencies
└── README.md # Documentation


---

## 🧠 Model Details
The model is a **Feedforward Artificial Neural Network (ANN)** trained for binary classification (Churn / No Churn).  
- **Activation Functions:** ReLU, Sigmoid  
- **Loss Function:** Binary Crossentropy  
- **Optimizer:** Adam  
- **Output:** Probability between 0 and 1  

---

## 💻 How to Run the Project

### 1️⃣ Clone the Repository
```bash
git clone https://github.com/<BUNNYBOBBALI>/customer-churn-prediction.git
cd customer-churn-prediction


2️⃣ Create a Virtual Environment
python -m venv .venv
# Activate venv
# Windows:
.venv\Scripts\activate
# macOS/Linux:
source .venv/bin/activate


3️⃣ Install Dependencies
pip install -r requirements.txt


4️⃣ Run the Streamlit App
streamlit run app.py
