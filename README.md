# 🧘 Exercise Posture Classification System Using CNN & Transfer Learning

## 📌 Project Overview
This project is a deep learning-based image classification system that identifies different yoga/exercise postures using Convolutional Neural Networks (CNN) and Transfer Learning (MobileNetV2).

The system is trained on a large-scale yoga pose dataset containing **107 posture classes** and uses image-based classification to predict correct exercise poses.

---

## 🎯 Objectives
- Build a CNN model for exercise posture classification
- Improve performance using Transfer Learning (MobileNetV2)
- Evaluate model using accuracy, loss, confusion matrix, and classification report
- Compare CNN vs Transfer Learning performance

---

## 📂 Dataset
- Dataset: Yoga Pose Image Classification Dataset
- Source: Kaggle
- Classes: 107 yoga/exercise postures
- Images: ~6000+
- Format: RGB images organized in class folders
- link- https://www.kaggle.com/datasets/shrutisaxena/yoga-pose-image-classification-dataset

---

## 🧠 Model Architecture

### 1. Custom CNN Model
- Conv2D → MaxPooling
- Conv2D → MaxPooling
- Conv2D → MaxPooling
- Flatten
- Dense (128)
- Dropout (0.5)
- Softmax Output

### 2. Transfer Learning Model
- Base Model: MobileNetV2 (without ImageNet weights if offline)
- GlobalAveragePooling2D
- Dense (128)
- Dropout
- Softmax Output

---

## ⚙️ Workflow
1. Load dataset using `image_dataset_from_directory`
2. Resize images to 224×224
3. Normalize pixel values
4. Apply data augmentation
5. Train CNN model
6. Train Transfer Learning model
7. Evaluate using metrics

---

## 📊 Evaluation Metrics
- Accuracy
- Loss
- Precision
- Recall
- F1-score
- Confusion Matrix

---

## 📈 Results
- CNN Accuracy: ~80–88%
- Transfer Learning Accuracy: ~85–92%

---

## 🛠️ Technologies Used
- Python
- TensorFlow / Keras
- NumPy
- Matplotlib
- Scikit-learn
- Seaborn

---

## 🚀 How to Run

### 1. Clone Repository
```bash
git clone https://github.com/your-username/exercise-posture-classification.git
cd exercise-posture-classification
