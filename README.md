# 🌦️ Weather Temperature Prediction using SimpleRNN (Deep Learning)

![Python](https://img.shields.io/badge/Python-3.9-blue)
![TensorFlow](https://img.shields.io/badge/TensorFlow-DeepLearning-orange)
![RNN](https://img.shields.io/badge/Model-RNN-green)
![Platform](https://img.shields.io/badge/Platform-Google%20Colab-yellow)

A deep learning project focused on building and evaluating a **Recurrent Neural Network (RNN)** using **SimpleRNN** for **time-series forecasting of daily temperature**.

---
# 📘 Project Overview

This project implements a **SimpleRNN model** to predict the **next day’s temperature** based on historical weather data.

The project covers the complete deep learning workflow including:

- Dataset exploration  
- Time-series preprocessing  
- Sequence creation  
- RNN model building  
- Model training and validation  
- Model evaluation  
- Future temperature forecasting  

The goal is to build a **robust time-series forecasting model using RNNs**.

---

# 🎯 Objective

The main objectives of this project are:

🔹 Understand time-series data  
🔹 Perform data preprocessing for sequential models  
🔹 Create input-output sequences for RNN  
🔹 Build a SimpleRNN model using TensorFlow/Keras  
🔹 Train the model  
🔹 Evaluate performance  
🔹 Forecast future temperature values  

---

# 📂 Dataset Information

The dataset used is the **Daily Weather Dataset** available on Kaggle.

Dataset Link:  
https://www.kaggle.com/datasets/muthuj7/weather-dataset

### Dataset Features

| Feature | Description |
|--------|------------|
| Date | Observation date |
| Temperature | Target variable |
| Humidity | Atmospheric humidity |
| Wind Speed | Wind velocity |
| Pressure | Atmospheric pressure (optional) |

---

# 🧹 Data Preprocessing

Before training the RNN model, several preprocessing steps were applied:

### ✔ Handling Missing Values
- Missing data was handled by removal or imputation.

### ✔ Normalization
- Data scaled using **MinMaxScaler** for faster convergence.

### ✔ Sequence Creation
- Input: Past **7–14 days of weather data**
- Output: **Next day temperature**

### ✔ Dataset Split
- Training Set  
- Validation Set  
- Test Set  

---

# 🧠 RNN Model Architecture

A **SimpleRNN model** was built using **TensorFlow / Keras**.

### Architecture Components

✔ Input Layer  
✔ SimpleRNN Layer (32–64 units)  
✔ Dropout Layer (optional)  
✔ Dense Output Layer (1 unit for regression)  

---

# ⚙ Model Training

The model was trained using the training dataset.

### Training Configuration

- Loss: Mean Squared Error (MSE)  
- Optimizer: Adam  
- Metrics: Mean Absolute Error (MAE)  
- Batch Size: 32  
- Epochs: 50–100  

### Monitoring

- Training Loss vs Validation Loss  
- Validation performance tracking  

---

# 📊 Model Evaluation

The model was evaluated on the test dataset.

### Evaluation Metrics

- RMSE  
- MAE  
- R² Score  

### Visualization

- Predicted vs Actual Temperature Plot  

---

# 🔮 Forecasting

The trained model was used to:

- Predict **next 7 days of temperature**
- Compare predictions with recent historical data  

---

# 🛠 Tech Stack

| Tool | Purpose |
|----|----|
| Python | Programming |
| TensorFlow / Keras | Deep Learning |
| NumPy | Numerical computation |
| Pandas | Data handling |
| Matplotlib | Visualization |
| Scikit-learn | Preprocessing & metrics |
| Kaggle API | Dataset download |
| Google Colab | Development |

---

# 📁 Repository Structure

```
weather-rnn-temperature-prediction/

│
├── DL_Assignment_2_RNN.ipynb
├── README.md
└── DL Assignment 2- RNN.pdf
```

---

# 🚀 How to Run the Project

### 1️⃣ Open the Notebook

Click the **Google Colab button above**.

---

### 2️⃣ Install Dependencies

```python
pip install tensorflow numpy pandas matplotlib scikit-learn kaggle
```

---

### 3️⃣ Kaggle API Setup

```python
!mkdir -p ~/.kaggle
!cp kaggle.json ~/.kaggle/
!chmod 600 ~/.kaggle/kaggle.json
```

Download dataset:

```python
!kaggle datasets download -d muthuj7/weather-dataset
```

Unzip:

```python
!unzip weather-dataset.zip
```

---

### 4️⃣ Run the Notebook

Run all cells to:

- Load dataset  
- Preprocess data  
- Create sequences  
- Train RNN model  
- Evaluate performance  
- Forecast temperatures  

---

# 🧠 Key Learning Outcomes

✔ Time-series forecasting  
✔ Sequence data preparation  
✔ RNN model building  
✔ Model evaluation  
✔ Future prediction using deep learning  

---

# 📌 Academic Submission

This project was developed as part of a **Deep Learning assignment** to demonstrate the implementation of a **SimpleRNN model for time-series temperature prediction**.
