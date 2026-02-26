
## PYTHON PROJECT -IMAGE CLASSIFICATION OF CATS AND DOGS USING CNN

##  👨‍💻 Author
Kshitij
Machine Learning Student
IBM Internship Project

## 🐶🐱 Dog vs Cat Image Classification using CNN (MobileNetV2)

This project is a Deep Learning Image Classification model that can identify whether an image contains a Dog or a Cat using a Convolutional Neural Network (CNN) with TensorFlow/Keras and MobileNetV2 transfer learning.

This project was developed as part of a Machine Learning / IBM Internship project.

---

## 📌 Project Overview

The main objectives of this project are:

- Build an accurate CNN model for image classification
- Use Transfer Learning (MobileNetV2)
- Train the model on Dogs vs Cats dataset
- Save the trained model for future predictions
- Predict whether an image is Dog or Cat

---

## 🧠 Technologies Used

- Python
- TensorFlow
- Keras
- CNN (Convolutional Neural Network)
- MobileNetV2 (Pretrained model)
- NumPy
- Matplotlib
- Jupyter Notebook / Google Colab

---

## 📂 Dataset

Dataset: Dogs vs Cats (Kaggle)

Structure:

dataset/
│
├── train/
│   ├── cat.0.jpg
│   ├── dog.0.jpg
│   └── ...
│
└── test/
    ├── cat.1000.jpg
    ├── dog.1000.jpg

Labels:

0 = Cat  
1 = Dog  

Total images: 25,000

---

## ⚙️ Model Architecture

MobileNetV2 (Pretrained)
↓
Global Average Pooling
↓
Dense Layer (ReLU)
↓
Output Layer (Softmax)

---

## 🏋️ Training Results

Training Accuracy: 97.7%  
Validation Accuracy: 97.3%  
Optimizer: Adam  
Loss Function: Sparse Categorical Crossentropy  

---

## 💾 Saved Model

dog_cat_M.h5

Load model example:

```python
from tensorflow.keras.models import load_model

model = load_model("dog_cat_M.h5")
