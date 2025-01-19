# **Electrocardiogram_Classifiers_LLNL**

This repository features the implementation of various machine learning models for classifying ECG (electrocardiogram) data, with a focus on detecting abnormalities and classifying different types of heartbeats. This project was hosted under Lawrence Livermore National Laboratory (LLNL) during the 2024 Data Science Challenge.

## **Table of Contents**

1. Binary Classification With Neural Network  
2. Binary Classification With Convolutional Neural Network  
3. Binary Classification With Decision Tree  
4. Multi-Class Classification With Neural Network  

## **Models Used**

1. **Neural Network (Binary Classification)**: A simple feedforward neural network for detecting normal and abnormal heartbeats.  
2. **Convolutional Neural Network (Binary Classification)**: A CNN designed to capture patterns in ECG signals for binary classification.  
3. **Decision Tree (Binary Classification)**: A traditional decision tree model for distinguishing between normal and abnormal heartbeats.  
4. **Neural Network (Multi-Class Classification)**: A neural network designed for classifying five types of heartbeats.  

## **Data**

### **Binary Classification Tasks**  
- **Dataset**: PTB Diagnostic ECG Database.  
- Labels:  
  - **0**: Normal heartbeats  
  - **1**: Abnormal heartbeats  

### **Multi-Class Classification Task**  
- **Dataset**: MIT-BIH Arrhythmia Database.  
- Labels:  
  - **0**: Normal (N)  
  - **1**: Supraventricular (S)  
  - **2**: Ventricular (V)  
  - **3**: Fusion (F)  
  - **4**: Unknown (Q)  

### **Preprocessing**
- All models utilize **SMOTE (Synthetic Minority Oversampling Technique)** to handle class imbalance in the dataset.

## **Installation**

To run the project locally, ensure you have Python 3.x installed along with the following libraries:  
- `torch` (PyTorch)  
- `scikit-learn`  
- `imbalanced-learn`  
- `matplotlib`  
- `seaborn`  

Install the required dependencies using pip:  
```bash

pip install torch scikit-learn imbalanced-learn matplotlib seaborn

```

## **Binary Classification Models**

### **Neural Network**
- **Architecture**: A feedforward neural network with hidden layers optimized using Adam optimizer and cross-entropy loss.  
- **Performance**: Achieved **93.16%** testing accuracy.  

### **Convolutional Neural Network**
- **Architecture**: A CNN model designed to extract spatial features from ECG data.  
- **Performance**: Achieved **91.92%** testing accuracy.  

### **Decision Tree**
- **Approach**: A traditional decision tree algorithm for binary classification.  
- **Performance**: Achieved **91.45%** testing accuracy.  

## **Multi-Class Classification Models**

### **Neural Network**
- **Architecture**: A feedforward neural network adapted for multi-class classification with one-hot encoded outputs.  
- **Performance**: Achieved **96.96%** testing accuracy.

## **How to Use**

1. Clone this repository to your local machine.
2. Ensure all dependencies are installed.
3. Run any of the Jupyter notebooks (`*.ipynb` files) to train and evaluate the models.
4. Feel free to experiment with hyperparameters or add your own features! Beware of a small learning rate, my computer almost exploded!

## **Contributions**

This project is part of my ongoing learning journey with machine learning. If you'd like to contribute, feel free to fork the repository and create a pull request with improvements or new models.

## **License**

This project is licensed under the MIT License.

## **Author**

Cristian Peña
