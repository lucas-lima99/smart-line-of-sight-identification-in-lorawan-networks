# LOS/NLOS Wireless Link Classification

This repository implements a **machine learning pipeline for classifying wireless communication links as Line-of-Sight (LOS) or Non-Line-of-Sight (NLOS)** using RSSI measurements and geographic information.

The project includes **data preprocessing, feature analysis, geographic visualization, and the evaluation of multiple machine learning algorithms**.

The goal is to investigate whether signal strength and spatial features can reliably determine the propagation condition of wireless links.

---

# Motivation

Wireless communication systems such as **LoRaWAN, cellular networks, and IoT deployments** are strongly affected by propagation conditions.

When a direct path exists between transmitter and receiver, the link operates under **Line-of-Sight (LOS)** conditions. However, in many environments (urban areas, forests, buildings), obstacles introduce **Non-Line-of-Sight (NLOS)** propagation.

Automatically identifying LOS/NLOS conditions is useful for:

- network planning
- propagation modeling
- link quality prediction
- adaptive communication strategies

This project explores a **data-driven approach using machine learning**.

---

# Workflow

The implemented pipeline follows these steps:

1. Dataset loading
2. LOS/NLOS labeling
3. Distance estimation relative to the gateway
4. Geographic visualization of measurements
5. Feature correlation analysis
6. Data preprocessing
7. Training multiple classification models
8. Cross-validation performance evaluation

---

# Dataset

Two datasets are used:

- **LOS measurements**
- **NLOS measurements**

# Machine Learning Models used

The notebook evaluates multiple classifiers.

### K-Nearest Neighbors (KNN)

A distance-based classifier that assigns labels based on neighboring samples.

### Multi-Layer Perceptron (MLP)

A neural network capable of modeling nonlinear relationships between features.

### Support Vector Machine (SVM)

A kernel-based method that constructs an optimal separating hyperplane.

### Random Forest (RF)

An ensemble of decision trees that improves classification stability and generalization.

---

# Model Evaluation

The models are evaluated using **10-fold cross-validation**

Evaluation metrics include:

- Accuracy
- Precision
- Recall
- F1-score
- Time

Author

Lucas Lima de Oliveira

Researcher in wireless communications, signal propagation, and machine learning for communication systems.
