# Intel Image Classification using CNN

A deep learning project for classifying images into **6 scene categories** using a custom Convolutional Neural Network (CNN) built with TensorFlow/Keras.

## 📌 Classes

* Buildings
* Forest
* Glacier
* Mountain
* Sea
* Street

## 🧠 Model

**Custom CNN Architecture:**

```text
Input (128×128×3)
       ↓
Conv2D (32) + ReLU
       ↓
Average Pooling
       ↓
Batch Normalization
       ↓
Dropout (0.3)
       ↓
Conv2D (64) + ReLU
       ↓
Average Pooling
       ↓
Batch Normalization
       ↓
Dropout (0.3)
       ↓
Flatten
       ↓
Dense (32) + ReLU
       ↓
Dropout
       ↓
Dense (6) + Softmax
```

## ⚙️ Configuration

* **Framework:** TensorFlow / Keras
* **Optimizer:** Adam
* **Loss:** Categorical Crossentropy
* **Epochs:** 20
* **Batch Size:** 50
* **Image Size:** 128×128
* **Normalization:** Pixel values scaled by `1/255`

## 📊 Results

| Metric              |  Score |
| ------------------- | -----: |
| Training Accuracy   | 87.55% |
| Validation Accuracy | 81.83% |
| Test Accuracy       |   ~82% |
| Macro F1-Score      |  ~0.82 |

The model was evaluated using **accuracy, precision, recall, F1-score, and a confusion matrix**.

## 📂 Dataset

**Intel Image Classification Dataset — Kaggle**

[Dataset on Kaggle](https://www.kaggle.com/datasets/puneet6060/intel-image-classification?utm_source=chatgpt.com)

The dataset contains approximately 25,000 images across the six scene categories.

## 🛠️ Technologies

* Python
* TensorFlow/Keras
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* Google Colab

## 🚀 Project Workflow


Dataset
  ↓
Image Preprocessing
  ↓
Custom CNN
  ↓
Model Training
  ↓
Validation
  ↓
Classification Report
  ↓
Confusion Matrix
  ↓
Prediction on New Images


