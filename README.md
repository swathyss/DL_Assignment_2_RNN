# 🌄 Intel Image Classification using CNN (Deep Learning)

![Python](https://img.shields.io/badge/Python-3.9-blue)
![TensorFlow](https://img.shields.io/badge/TensorFlow-DeepLearning-orange)
![CNN](https://img.shields.io/badge/Model-CNN-green)
![Platform](https://img.shields.io/badge/Platform-Google%20Colab-yellow)

A deep learning project focused on building and evaluating a **Convolutional Neural Network (CNN)** for **multi-class image classification** using the **Intel Image Classification dataset**.

---

## 🚀 Run Notebook in Google Colab

Click the button below to open the notebook directly in Google Colab.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Laya123-star/intel-image-classification-cnn/blob/main/DL_Assignment_1_CNN.ipynb)

---

# 📘 Project Overview

This project implements a **Convolutional Neural Network (CNN)** to classify natural scene images into multiple categories.

The project covers the complete deep learning pipeline including:

- Dataset exploration  
- Image preprocessing  
- Data augmentation  
- CNN architecture design  
- Model training and validation  
- Model evaluation using performance metrics  
- Prediction visualization  

The goal is to build a **robust CNN model capable of accurately classifying real-world natural scenes**.

---

# 🎯 Objective

The main objectives of this project are:

🔹 Understand the structure of an image dataset  
🔹 Perform image preprocessing and augmentation  
🔹 Build a CNN architecture from scratch  
🔹 Train the model using TensorFlow/Keras  
🔹 Evaluate model performance using multiple metrics  
🔹 Visualize model predictions on unseen test images  

---

# 📂 Dataset Information

The dataset used is the **Intel Image Classification Dataset** available on Kaggle.

Dataset Link:  
https://www.kaggle.com/datasets/puneet6060/intel-image-classification

### Dataset Details

| Feature | Description |
|------|-------------|
| Total Images | 25,000+ |
| Image Type | Natural Scene Images |
| Number of Classes | 6 |
| Image Size | Resized to 150 × 150 |

### Target Classes

The dataset contains **6 scene categories**:

- 🏢 Buildings  
- 🌲 Forest  
- 🧊 Glacier  
- ⛰ Mountain  
- 🌊 Sea  
- 🛣 Street  

---

# 🧹 Data Preprocessing

Before training the CNN model, several preprocessing steps were applied:

### ✔ Image Resizing
All images were resized to **150 × 150 pixels** to maintain uniform input size.

### ✔ Pixel Normalization
Pixel values were scaled to the range **0–1** by dividing by 255.

### ✔ Train / Validation / Test Split
The dataset was split into:

- Training Set  
- Validation Set  
- Test Set  

### ✔ Data Augmentation

To improve model generalization and prevent overfitting, the following augmentation techniques were used:

- Image Rotation  
- Horizontal Flip  
- Zoom  
- Width & Height Shift  
- Shear Transform  

---

# 🧠 CNN Model Architecture

A **Convolutional Neural Network (CNN)** was built from scratch using **TensorFlow / Keras**.

### Architecture Components

✔ Convolutional Layers  
✔ ReLU Activation Function  
✔ Max Pooling Layers  
✔ Dropout Layers for Regularization  
✔ Fully Connected (Dense) Layers  
✔ Softmax Output Layer for Multi-Class Classification  

---

# ⚙ Model Training

The CNN model was trained using the **training dataset** and validated using the **validation dataset**.

### Training Techniques Used

- Early Stopping  
- Model Checkpointing  
- Batch Training  
- Validation Monitoring  

Training progress was monitored using:

- Training Accuracy vs Validation Accuracy  
- Training Loss vs Validation Loss  

---

# 📊 Model Evaluation

After training, the model was evaluated using the **test dataset**.

### Evaluation Metrics

- Accuracy  
- Precision  
- Recall  
- F1 Score  
- Confusion Matrix  

---

# 🔍 Prediction Visualization

To better understand the model’s performance:

- **10 random test images** were selected
- Each image was displayed with:
  - Actual Label
  - Predicted Label

---

# 🛠 Tech Stack

| Tool | Purpose |
|----|----|
| Python | Programming language |
| TensorFlow / Keras | Deep learning framework |
| NumPy | Numerical computation |
| Matplotlib | Visualization |
| Seaborn | Confusion matrix visualization |
| OpenCV / PIL | Image processing |
| Kaggle API | Dataset download |
| Google Colab | Development environment |

---

# 📁 Repository Structure

```
intel-image-classification-cnn/

│
├── DL_Assignment_1_CNN.ipynb
├── README.md
└── DL Assignment 1 - CNN.pdf
```

---

# 🚀 How to Run the Project

### 1️⃣ Open the Notebook

Click the **Google Colab button above**.

---

### 2️⃣ Install Required Libraries

```python
pip install tensorflow matplotlib numpy seaborn kaggle
```

---

### 3️⃣ Kaggle API Setup

Upload your **kaggle.json** file and run:

```python
!mkdir -p ~/.kaggle
!cp kaggle.json ~/.kaggle/
!chmod 600 ~/.kaggle/kaggle.json
```

Download dataset:

```python
!kaggle datasets download -d puneet6060/intel-image-classification
```

Unzip dataset:

```python
!unzip intel-image-classification.zip
```

---

### 4️⃣ Run the Notebook

Run all cells sequentially to:

- Load dataset
- Preprocess images
- Train CNN model
- Evaluate performance
- Visualize predictions

---

# 🧠 Key Learning Outcomes

✔ Understanding CNN architecture  
✔ Image preprocessing techniques  
✔ Data augmentation for deep learning  
✔ Training deep learning models  
✔ Evaluating classification performance  
✔ Visualizing CNN predictions  

---

# 📌 Academic Submission

This repository was created as part of a **Deep Learning assignment** to demonstrate the design, training, and evaluation of a **Convolutional Neural Network (CNN)** for real-world image classification.