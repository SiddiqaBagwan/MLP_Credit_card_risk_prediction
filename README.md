# Credit Risk Prediction using Multi-Layer Perceptron (MLP)

A deep learning-based credit risk prediction system developed using a **Multi-Layer Perceptron (MLP)** to classify customers as **Good Credit** or **Bad Credit** using the **German Credit Dataset**.

This project demonstrates the complete deep learning pipeline including data preprocessing, feature encoding, feature scaling, model training, evaluation, and visualization of performance metrics.

---

## 📌 Objective

The objective of this project is to predict whether a loan applicant belongs to the **Good Credit** or **Bad Credit** category based on customer financial and demographic information.

The model is implemented using **TensorFlow/Keras** and evaluated using multiple performance metrics including Accuracy, Precision, Recall, F1-score, and Confusion Matrix.

---

## 📂 Dataset

**Dataset:** German Credit Dataset

- Total Records: **1000**
- Total Features: **20 Input Features + 1 Target Column**
- Target Classes:
  - **1 → Good Credit**
  - **0 → Bad Credit**

---

# 🛠 Technologies Used

- Python
- NumPy
- Pandas
- TensorFlow / Keras
- Scikit-learn
- Matplotlib

---

# ⚙️ Data Preprocessing

The following preprocessing steps were performed:

- Loaded the German Credit Dataset
- Label Encoding for categorical features
- Feature Scaling using **StandardScaler**
- Train-Test Split (80:20)
- Stratified Sampling
- Random State = 42

---

# 🧠 Model Architecture

```
Input Layer (20 Features)
        │
        ▼
Dense Layer (32 Neurons)
Activation: ReLU
        │
        ▼
Dropout (0.3)
        │
        ▼
Dense Layer (16 Neurons)
Activation: ReLU
        │
        ▼
Dropout (0.3)
        │
        ▼
Output Layer (1 Neuron)
Activation: Sigmoid
```

---

# ⚙️ Model Configuration

| Parameter | Value |
|-----------|-------|
| Optimizer | Adam |
| Loss Function | Binary Crossentropy |
| Activation (Hidden Layers) | ReLU |
| Activation (Output Layer) | Sigmoid |
| Batch Size | 32 |
| Maximum Epochs | 30 |
| Validation Split | 20% |
| EarlyStopping | Enabled |

---

# 📈 Training

The model was trained using:

- Adam Optimizer
- Binary Crossentropy Loss
- EarlyStopping
- Validation Split = 20%

During training, the following were monitored:

- Training Accuracy
- Validation Accuracy
- Training Loss
- Validation Loss

---

# 📊 Results

## Test Accuracy

**72.50%**

```
Test Accuracy: **0.7250000238418579**
```

---

## Classification Performance

| Metric | Score |
|---------|------:|
| Accuracy | **72.5%** |
| Precision | **≈76%** |
| Recall | **≈89%** |
| F1-Score | **≈82%** |

---

## Confusion Matrix

```
                 Predicted

              Bad     Good

Actual Bad      21      39
Actual Good     15     125
```

Where:

- **TP = 125**
- **TN = 21**
- **FP = 39**
- **FN = 15**

---

# 📉 Evaluation Metrics

The model performance was evaluated using:

- Accuracy
- Precision
- Recall
- F1-score
- Confusion Matrix
- Classification Report

---

# 📈 Training Visualizations

The project includes:

- Accuracy vs Epoch Graph
- Validation Accuracy Graph
- Loss vs Epoch Graph
- Validation Loss Graph

These graphs help visualize the learning process and monitor overfitting.

---

# 📌 Project Workflow

```
Load Dataset
      │
      ▼
Data Preprocessing
(Label Encoding)
      │
      ▼
Feature Scaling
(StandardScaler)
      │
      ▼
Train-Test Split
      │
      ▼
Build MLP Model
      │
      ▼
Compile Model
(Adam + Binary Crossentropy)
      │
      ▼
Train Model
(model.fit)
      │
      ▼
Evaluate Model
(model.evaluate)
      │
      ▼
Generate Predictions
      │
      ▼
Confusion Matrix
      │
      ▼
Classification Report
      │
      ▼
Performance Graphs
```

---

# 🎯 Key Features

- Credit Risk Prediction using Deep Learning
- Multi-Layer Perceptron (MLP)
- StandardScaler for feature normalization
- Label Encoding for categorical variables
- EarlyStopping to reduce overfitting
- Adam Optimizer
- Binary Classification
- Performance visualization using graphs

---

# 📚 Learning Outcomes

Through this project, the following concepts were implemented and understood:

- Artificial Neural Networks (ANN)
- Multi-Layer Perceptron (MLP)
- Dense Layers
- ReLU Activation
- Sigmoid Activation
- Dropout Regularization
- Binary Crossentropy Loss
- Adam Optimizer
- Forward Propagation
- Backpropagation
- StandardScaler
- Label Encoding
- Train-Test Split
- Stratified Sampling
- EarlyStopping
- Accuracy, Precision, Recall & F1-score
- Confusion Matrix
- Model Evaluation

---

# 🚀 Future Improvements

- Hyperparameter tuning
- Experiment with different optimizers
- Cross-validation
- Feature engineering
- Compare MLP with other machine learning algorithms such as Random Forest, XGBoost, and SVM.

---

# 📄 Conclusion

A Multi-Layer Perceptron (MLP) model was successfully implemented to classify customers into **Good Credit** and **Bad Credit** categories using the German Credit Dataset. The model achieved a **test accuracy of 72.5%** with strong recall (≈89%) and balanced overall performance. The project demonstrates the complete workflow of building, training, and evaluating a deep learning model for binary classification in credit risk prediction.
