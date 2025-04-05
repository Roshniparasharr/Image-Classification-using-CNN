# Image Classification - Cats vs Dogs (CNN | TensorFlow | KaggleHub)

This project implements an end-to-end **Image Classification** system using a **Convolutional Neural Network (CNN)** built with **TensorFlow/Keras** to distinguish between cats and dogs. The dataset is sourced from **KaggleHub** and consists of 25,000 labeled images split into training and testing sets.

## 📌 Key Highlights

- ✅ Dataset: [Dogs vs Cats Dataset](https://www.kaggle.com/datasets/salader/dogs-vs-cats) via `kagglehub`
- ✅ Preprocessing: Resizing, normalization, batching using `image_dataset_from_directory()`
- ✅ Architecture: Multi-layer CNN with `Conv2D`, `BatchNormalization`, `MaxPooling2D`, and `Dropout`
- ✅ Loss Function: `Binary Crossentropy`
- ✅ Optimizer: `Adam`
- ✅ Evaluation Metrics: Accuracy, Loss (Train & Validation)
- ✅ Custom image prediction support

## 🧠 CNN Model Summary

```plaintext
Conv2D(32) → BN → MaxPool
Conv2D(64) → BN → MaxPool
Conv2D(128) → BN → MaxPool
Flatten → Dense(128) → Dropout → Dense(64) → Dropout → Dense(1, sigmoid)
```

## 📊 Performance

- Achieved ~73% validation accuracy within just 3 epochs
- Training and validation curves plotted for analysis
- Real-time inference on uploaded images

## 🖼️ Demo

```python
Input: /content/images.jpeg
Prediction: Dog 🐶 (Probability > 0.5)
```

## 🧪 Libraries Used

- TensorFlow / Keras
- OpenCV
- Matplotlib
- KaggleHub
- Python 3.x

---

