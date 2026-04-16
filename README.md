# Lung Cancer Detection using Deep Learning

## Project Overview

This project explores the application of deep learning techniques for lung CT scan image classification using Convolutional Neural Networks (CNNs).

The goal of the project is to build an end-to-end workflow that can classify lung CT scan images and demonstrate how deep learning models can learn visual features from medical imaging data.

Two versions of the model were developed:

• **Binary Classification Model**  
Classifies CT scans as **Cancer** or **Normal**

• **Multi-Class Classification Model**  
Classifies CT scans into:

- Benign  
- Malignant  
- Normal  

This project demonstrates a **proof-of-concept deep learning workflow**, including data preprocessing, CNN model development, training, evaluation, and visualization of model predictions.

---

# Dataset

The dataset used in this project is the **IQ-OTHNCCD Lung Cancer Dataset**, which contains CT scan images categorized into three classes.

### Classes

• **Normal** – CT scans without lung cancer  
• **Benign** – Non-cancerous lung abnormalities  
• **Malignant** – Cancerous lung tumors  

### Dataset Characteristics

- CT scan images
- Class-labeled folders
- Used for image classification experiments
- Preprocessed and resized before model training

All images were converted to grayscale and resized to **128 × 128 pixels** before training.

---

# Tools & Technologies

This project uses the following tools and libraries:

**Programming Language**
- Python

**Deep Learning Framework**
- TensorFlow
- Keras

**Data Processing**
- NumPy
- OpenCV

**Visualization**
- Matplotlib
- Seaborn

**Machine Learning Utilities**
- Scikit-learn

**Development Environment**
- Jupyter Notebook

---

# Project Workflow

The overall workflow of the project includes:

1. Dataset preparation and folder organization
2. Image preprocessing using OpenCV
3. Image resizing and normalization
4. Train-test dataset splitting
5. CNN architecture development
6. Model training using TensorFlow/Keras
7. Model evaluation
8. Visualization of training results
9. Prediction on CT scan images
10. Saving trained models

---

# CNN Model Architecture

The CNN architecture includes:

- Convolution Layers
- MaxPooling Layers
- Flatten Layer
- Dense Layers
- Dropout Layer
- Output Layer

The model learns visual patterns from CT scan images and uses these learned features to classify lung conditions.

---

## Results

The advanced CNN model demonstrates a proof-of-concept workflow for multi-class classification of lung CT scan images using the current dataset split.

The following visualizations summarize model training behavior and prediction outputs.

---

### Training Accuracy

![Training Accuracy](images/training_accuracy.png)

This graph shows how training and validation accuracy changed during model training on the current dataset split.

---

### Training Loss

![Training Loss](images/training_loss.png)

This graph shows how training and validation loss changed across training epochs.

---

### Confusion Matrix

![Confusion Matrix](images/confusion_matrix.png)

The confusion matrix summarizes prediction results across the **Benign**, **Malignant**, and **Normal** classes.

---

### Prediction Distribution

![Prediction Distribution](images/prediction_distribution.png)

This chart shows how many images were predicted for each class by the trained CNN model.

---


## Limitations

This project is intended as a proof-of-concept deep learning workflow for medical image classification.

The current results are based on a dataset-specific train-test split and do not include external validation, patient-level splitting, or clinical testing.

Therefore, the results should not be interpreted as medical diagnostic performance.
---

# Project Structure
Lung-Cancer-Detection
│
├── images
│ ├── training_accuracy.png
│ ├── training_loss.png
│ ├── confusion_matrix.png
│ ├── prediction_distribution.png
│ ├── prediction_normal.png
│ └── prediction_malignant.png

├── Notebook
│ ├── basic_cnn_lung_cancer_detection.ipynb
│ └── advanced_lung_cancer_detection.ipynb

├── models
│ ├── lung_cancer_cnn_model.keras
│ └── advanced_lung_cancer_model.keras

├── index.html
├── style.css
├── README.md
