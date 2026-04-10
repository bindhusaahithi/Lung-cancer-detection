# Lung Cancer Detection using Deep Learning

## Project Overview
This project uses Convolutional Neural Networks (CNNs) to classify lung CT scan images.

Two versions of the project were developed:
- **Basic CNN Model**: Binary classification (`Cancer` vs `Normal`)
- **Advanced CNN Model**: Multi-class classification (`Benign`, `Malignant`, `Normal`)

## Dataset Structure

### Basic Dataset
- `Data/cancer`
- `Data/normal`

### Advanced Dataset
- `Data_3class/benign`
- `Data_3class/malignant`
- `Data_3class/normal`

## Project Workflow
1. Organize CT scan images into class-based folders
2. Preprocess images using OpenCV
3. Resize images to `128x128`
4. Normalize pixel values
5. Split data into training and testing sets
6. Build CNN model
7. Train and evaluate the model
8. Save trained models for later use
9. Load the saved models and make predictions

## Models
- `lung_cancer_cnn_model.keras` → Basic binary CNN model
- `advanced_lung_cancer_model.keras` → Advanced multi-class CNN model

## Technologies Used
- Python
- TensorFlow / Keras
- OpenCV
- NumPy
- Matplotlib
- Scikit-learn

## Notebooks
- `basic_cnn_lung_cancer_detection.ipynb`
- `advanced_lung_cancer_detection.ipynb`

## Results
The project demonstrates lung CT scan classification using deep learning and includes prediction examples from trained models.

## Future Improvements
- Add transfer learning models
- Use larger medical imaging datasets
- Deploy the model using Streamlit or Flask

## Example Predictions

Below are example predictions from the trained CNN model.

### Normal Lung CT Scan

![Normal Prediction](images/prediction_normal.png)

Model Prediction: **Normal**

---

### Malignant Lung CT Scan

![Malignant Prediction](images/prediction_malignant.png)

Model Prediction: **Malignant**
