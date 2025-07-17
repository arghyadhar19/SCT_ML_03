# SCT_ML_03

# 🐶🐱 Dog vs. Cat Image Classifier using HOG + PCA + SVM

This project demonstrates how to classify images of **dogs and cats** using **HOG (Histogram of Oriented Gradients)** features, **PCA (Principal Component Analysis)** for dimensionality reduction, and **SVM (Support Vector Machine)** for classification.

## 📂 Dataset

[Dogs vs. Cats](https://www.kaggle.com/c/dogs-vs-cats/data).
The training dataset must follow this structure:
dogs-vs-cats (1)/
└── train/
└── train/
├── cat.0.jpg
├── dog.0.jpg
└── ...

Test images should be placed in:
/kaggle/input/dog-cat-test/
└── image1.jpg
└── image2.jpg


> 📝 Only images starting with `cat` or `dog` are processed in training.

---

## 📌 Features

- 📷 **Grayscale HOG Feature Extraction**
- 📉 **PCA** to retain 95% variance
- 🤖 **SVM (RBF Kernel)** with GridSearchCV
- 📊 Confusion Matrix, Classification Report
- 🧪 Predict unseen test images with confidence scores

---

## 🔧 Setup

```bash
pip install numpy opencv-python matplotlib seaborn scikit-learn scikit-image tqdm
