# 🐱🐶 Cats vs Dogs Image Classifier using Convolutional Neural Networks (CNN)

A Deep Learning based image classification project that accurately distinguishes between **Cats** and **Dogs** using a **Convolutional Neural Network (CNN)** built with **TensorFlow** and **Keras**.

The model is trained on the **Dogs vs Cats** dataset from Kaggle and is capable of predicting completely unseen images with good classification performance.

---

## 📌 Project Overview

Image classification is one of the most fundamental applications of Deep Learning and Computer Vision. This project demonstrates how a CNN can automatically learn visual features from images and classify them into two categories:

- 🐱 Cat
- 🐶 Dog

The complete pipeline includes:

- Data preprocessing
- CNN model development
- Model training
- Performance evaluation
- Prediction on unseen images

---

## 🎯 Objectives

- Learn the fundamentals of Convolutional Neural Networks.
- Build an end-to-end image classification model.
- Understand feature extraction using convolution layers.
- Prevent overfitting using Batch Normalization and Dropout.
- Evaluate model performance using validation accuracy and loss.
- Predict real-world images that were never seen during training.

---

# 🛠️ Tech Stack

| Category | Technology |
|----------|------------|
| Language | Python |
| Deep Learning | TensorFlow |
| Neural Network API | Keras |
| Dataset Download | KaggleHub |
| Development Environment | Jupyter Notebook |

---

# 📂 Dataset

**Dataset Name**

Dogs vs Cats Dataset

Source:

https://www.kaggle.com/datasets/salader/dogsvscats

### Dataset Information

- Total Images: **25,000**
- Classes: **2**
- Cat Images
- Dog Images

Images were resized to:

```
64 × 64 × 3
```

before training.

---

# ⚙️ Data Preprocessing

The dataset was prepared using **ImageDataGenerator**.

The preprocessing pipeline includes:

- Image Rescaling
- Training Dataset Generation
- Validation Dataset Generation
- Batch Loading

---

# 🧠 CNN Architecture

The CNN consists of three major stages:

## Feature Extraction

### Convolution Block 1

- Conv2D (32 Filters)
- ReLU Activation
- Batch Normalization
- MaxPooling

### Convolution Block 2

- Conv2D (64 Filters)
- ReLU Activation
- Batch Normalization
- MaxPooling

### Convolution Block 3

- Conv2D (128 Filters)
- ReLU Activation
- Batch Normalization
- MaxPooling

These convolution layers progressively learn:

- Edges
- Shapes
- Textures
- Complex image patterns

---

## Flatten Layer

The extracted feature maps are converted into a one-dimensional feature vector before entering the classifier.

---

## Classification Network

Dense Layer (128)

↓

Batch Normalization

↓

Dropout (0.5)

↓

Dense Layer (64)

↓

Batch Normalization

↓

Dropout (0.3)

↓

Output Layer (1 Neuron)

↓

Sigmoid Activation

---

# 🚀 Model Compilation

Optimizer

```
Adam
```

Loss Function

```
Binary Crossentropy
```

Evaluation Metric

```
Accuracy
```

---

# 📈 Training Strategy

To improve model performance, the following techniques were used:

### ✅ Batch Normalization

- Stabilizes learning
- Faster convergence
- Reduces Vanishing Gradient Problem

### ✅ Dropout

Randomly disables neurons during training to reduce overfitting.

### ✅ Pyramid Dense Layers

The Dense layers gradually decrease in size:

```
128

↓

64

↓

1
```

which improves feature learning.

### ✅ Early Stopping

Stops training automatically when the validation loss stops improving.

This prevents unnecessary training and reduces overfitting.

---

# 📊 Model Performance

The model was evaluated using:

- Training Accuracy
- Validation Accuracy
- Training Loss
- Validation Loss

### Training Graphs

(Add screenshots here)

```
screenshots/training_accuracy.png
```

```
screenshots/training_loss.png
```

---

# 🔍 Prediction on Unseen Images

After training, the model was tested using completely new images that were never used during training.

Example Predictions

| Image | Prediction |
|--------|------------|
| Cat Image | 🐱 Cat |
| Dog Image | 🐶 Dog |

---

# 📸 Project Demo

https://github.com/user-attachments/assets/a0fbada6-f716-47dd-bbbd-cefffd11e83e

---

# ▶️ How to Run

### Clone the repository

```bash
git clone https://github.com/ManthanTerse/Cats-vs-Dogs-Image-Classifier-using-CNN.git
```

Move into the project

```bash
cd Cats-vs-Dogs-Image-Classifier
```

Install dependencies

```bash
pip install -r requirements.txt
```

Open

```
cats_vs_dogs_classifier.ipynb
```

Run all cells.

---

# 💡 Future Improvements

- Transfer Learning using VGG16
- MobileNet
- ResNet50
- EfficientNet
- Hyperparameter Tuning
- Data Augmentation
- Model Deployment using Streamlit
- Flask API Integration
- Docker Support

---

# 📚 Learning Outcomes

Through this project, I learned:

- Convolutional Neural Networks
- Image Preprocessing
- Binary Image Classification
- Feature Extraction
- Batch Normalization
- Dropout Regularization
- Early Stopping
- TensorFlow & Keras Workflow
- Model Evaluation
- Prediction on Real-world Images

---

# 🙋‍♂️ Author

**Manthan Terse**

Artificial Intelligence & Data Science Student

LinkedIn: https://linkedin.com/in/manthanterse

---

# ⭐ If you found this project helpful, consider giving it a Star!
