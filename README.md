# 🍅 Tomato Leaf Disease Detection & Classification

A **Deep Learning–based Computer Engineering project** focused on accurate and efficient classification of tomato leaf diseases.
The system is designed to deliver **high predictive performance while remaining computationally lightweight and environmentally conscious (Green AI approach).**

---

## 🌟 Key Features

### ✅ Multi-Class Disease Classification

Detects and classifies multiple tomato plant health conditions:

* Bacterial Spot
* Early Blight
* Late Blight
* Tomato Yellow Leaf Curl Virus
* Healthy Leaves

### ⚙️ Optimized CNN Architecture

* Custom **Convolutional Neural Network (CNN)** tailored for plant pathology recognition
* Strong spatial feature extraction with **low parameter overhead**
* Designed for **efficient training on limited hardware**

### 🧠 Memory-Efficient Training Pipeline

* Built to handle **RAM constraints during training**
* Uses **on-the-fly augmentation** instead of dataset expansion

### 🚀 Efficient Data Pipeline

* Implemented with **TensorFlow tf.data API**
* Uses:

  * Prefetching
  * Caching
  * Parallel data loading
* Maximizes **GPU utilization and training throughput**

### 🌱 Green AI Approach

* Reduced computational cost via:

  * Early stopping
  * Efficient image resizing
  * Lightweight augmentation strategy

---

## 📊 Model Performance

| Metric              | Result                                      |
| ------------------- | ------------------------------------------- |
| Validation Accuracy | ~98%                                        |
| Loss Function       | Categorical Cross-Entropy                   |
| Evaluation Strategy | Validation-set based performance monitoring |

The model demonstrates **robust generalization across disease classes**, making it suitable for practical agricultural applications.

---

## 📁 Project Structure

```
tomato-disease-detection/
│
├── notebook/
│   └── training.ipynb        # Training pipeline, EDA, evaluation
│
├── models/                   # Saved trained models (.h5 / .keras)
│
├── .gitignore
└── README.md
```

---

## 🛠️ Tech Stack

**Deep Learning Framework**

* TensorFlow
* Keras

**Supporting Libraries**

* NumPy
* Pandas
* Matplotlib
* OpenCV

**Development Environment**

* Jupyter Notebook
* Google Colab

---

## ⚙️ Implementation Details

### 📐 Image Preprocessing

All images are resized to **256 × 256 pixels** to balance:

* Fine-grained disease texture preservation
* Computational efficiency
* Memory optimization

### 🔄 Strategic Data Augmentation

A **minimal yet effective augmentation strategy** was used:

* Random Horizontal & Vertical Flips
* Random Rotation

These augmentations are applied **dynamically during training**, reducing memory usage while improving generalization.

---

## 🚀 Future Enhancements

* 🌐 **API Deployment**
  Integrate with FastAPI for real-time disease prediction via web interface

* 📱 **Mobile Optimization**
  Convert model to **TensorFlow Lite (TFLite)** for offline rural deployment

* 📡 **Edge AI Integration**
  Deploy on **IoT-enabled smart cameras** for automated greenhouse monitoring

---

## 📊 Dataset Credit

This project uses the **PlantVillage Dataset**:
https://www.kaggle.com/datasets/arjuntejaswi/plant-village/data

All dataset rights belong to the original creators and contributors.

---

## 👨‍💻 Author

**Sandeep**
🔗 GitHub: https://github.com/sandeepdgn
**Prithak**
🔗 GitHub: https://github.com/sasquatchrex
**Diwen**
🔗 GitHub: https://github.com/squareshot-db
---

## ⭐ Project Goal

To build a **practical, scalable, and environmentally responsible AI system** that supports farmers and agricultural researchers in **early detection of crop diseases**, ultimately contributing to improved food security.

---
