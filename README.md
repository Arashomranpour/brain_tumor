<div align="center">

# 🧠 Brain Tumor MRI Classification

**A convolutional neural network (Keras / TensorFlow) that classifies brain MRI scans into four categories.**

![Python](https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white)
![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?logo=tensorflow&logoColor=white)
![Keras](https://img.shields.io/badge/Keras-D00000?logo=keras&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?logo=jupyter&logoColor=white)

</div>

---

## ✨ Overview

The notebook trains an image classifier on brain MRI images with four classes:

| Class |
|---|
| 🟠 `glioma_tumor` |
| 🟡 `meningioma_tumor` |
| 🟢 `no_tumor` |
| 🔵 `pituitary_tumor` |

**Pipeline**

1. Load images from class folders, resize and convert them to NumPy arrays.
2. Split into train and validation sets.
3. Train a CNN with four `Conv2D` blocks (32 → 64 → 128 → 256 filters) for up to 50 epochs.
4. Evaluate accuracy and predict on new images.

**Training progress:** validation accuracy rose from ~62 % in the first epoch to roughly **87-88 %** in the later epochs recorded in the notebook.

> ⚠️ Educational project - not a medical device.

## 🚀 Getting Started

Open `brain_tumor.ipynb` in [Google Colab](https://colab.research.google.com/) (a GPU is recommended) or locally:

```bash
git clone https://github.com/Arashomranpour/brain_tumor.git
cd brain_tumor
pip install tensorflow keras opencv-python pillow scikit-learn pandas matplotlib tqdm jupyter
jupyter notebook brain_tumor.ipynb
```

The notebook expects a brain-tumor MRI dataset organised in one folder per class (for example the public Kaggle *Brain Tumor Classification (MRI)* dataset); update the path in the data-loading cell.

## 📁 Project Structure

```
.
└── brain_tumor.ipynb     # Data prep, CNN, training and evaluation
```

## 🛠️ Tech Stack

`TensorFlow` · `Keras` · `OpenCV` · `scikit-learn` · `NumPy` · `Matplotlib`
