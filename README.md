#  Fraud Detection AI

A powerful deep learning system for detecting fraudulent transactions using a combination of Dense Neural Networks, LSTM for sequence modeling, and Autoencoder for anomaly detection.

---

##  Overview

Fraudulent activity detection is critical in modern finance. This project applies deep learning techniques to identify suspicious transactions based on patterns in time-series and tabular data.

The system supports three key model architectures:

- **Dense Neural Network (DNN)** – for basic classification
- **LSTM** – for sequence-aware transaction modeling
- **Autoencoder** – for unsupervised anomaly detection

---

##  Model Architectures

### 1. Dense Neural Network (DNN)
A fully connected feedforward network for binary classification of transactions.

- Input: Tabular transaction data
- Layers: Dense + ReLU + Dropout
- Output: Sigmoid (fraud / not fraud)

### 2. LSTM
Captures temporal dependencies in user behavior and transaction patterns.

- Input: Sequences of transactions per user
- Layers: LSTM + Dense
- Output: Sigmoid fraud prediction

### 3. Autoencoder
Learns the normal pattern of transactions; high reconstruction error indicates potential fraud.

- Input: Normal transaction data only
- Layers: Encoder → Bottleneck → Decoder
- Output: Reconstruction loss used as fraud signal


