# 🌍 Federated Learning-Based ANN for Distributed Air Quality Prediction

## 📌 Overview

Air pollution is a critical environmental issue that directly impacts public health and climate. Traditional air quality prediction methods rely on **centralized data collection**, which can be inefficient, privacy-invasive, and limited in scalability.

This project introduces a **Federated Learning (FL)** framework integrated with an **Artificial Neural Network (ANN)** to predict air pollutant levels across distributed nodes (e.g., multiple cities, stations, or IoT devices). Instead of transferring sensitive local data, the model learns collaboratively, preserving **data privacy** while improving **accuracy and generalization**.

The project can be used as a foundation for:

* **Smart city monitoring systems**
* **Environmental research studies**
* **IoT-enabled pollution sensing networks**
* **Privacy-preserving collaborative research**

---

## 🎯 Objectives

* ✅ Implement a **Federated Learning framework** for air quality prediction
* ✅ Train an **ANN model** on distributed client datasets
* ✅ Aggregate local models to improve prediction accuracy
* ✅ Compare **federated vs centralized training approaches**
* ✅ Provide visualizations & performance metrics for evaluation

---

## 🚀 Features

* 🔐 **Privacy-preserving** training using Federated Learning
* 🧠 ANN-based regression/classification for pollutant levels
* 📊 Data preprocessing & feature scaling
* ⚡ Model evaluation with metrics (RMSE, MAE, R²)
* 🌐 Scalable design: add more clients with minimal setup
* 📉 Visualization of predictions vs actual values
* 🏗️ Modular code structure for easy extension

---

## 📂 Repository Structure

```
federated-air-quality-prediction/
│
├── data/                   # Sample or preprocessed datasets (small files only)
│   └── data_air_pollutant.csv
│
├── notebooks/              # Jupyter notebooks for experiments
│   └── exploratory_analysis.ipynb
│
├── src/                    # Source code
│   ├── preprocessing.py    # Data cleaning & scaling
│   ├── model.py            # ANN model definition
│   ├── federated.py        # Federated learning aggregation logic
│   ├── train.py            # Training script
│   └── main.py             # Entry point for running the project
│
├── models/                 # Saved models/checkpoints
│   └── model_weights.h5
│
├── results/                # Graphs, performance metrics, reports
│   └── evaluation.png
│
├── requirements.txt        # Python dependencies
├── environment.yml         # (optional) Conda environment
├── README.md               # Project documentation
├── .gitignore              # Ignore unnecessary files
└── LICENSE                 # License file
```

---

## ⚙️ Installation

### 🔹 Clone the repository

```bash
git clone https://github.com/yourusername/federated-air-quality-prediction.git
cd federated-air-quality-prediction
```

### 🔹 Install dependencies

```bash
pip install -r requirements.txt
```

Or with Conda:

```bash
conda env create -f environment.yml
conda activate air-quality-fl
```

---

## ▶️ Usage

### Train the model centrally (baseline)

```bash
python src/train.py --mode centralized
```

### Train the model with Federated Learning

```bash
python src/main.py --clients 5 --rounds 20
```

### Run Jupyter Notebook experiments

```bash
jupyter notebook notebooks/
```

---

## 📊 Results & Evaluation

* Federated Learning improves prediction robustness across distributed nodes

* Performance Metrics:

  * **RMSE**: 2.31
  * **MAE**: 1.74
  * **R² Score**: 0.89

* Visualization of **Predicted vs Actual pollutant levels**:
  ![Results Graph](results/evaluation.png)

---

## 🔮 Future Work

* 🌐 Extend to **Bayesian Neural Networks (BNNs)** for uncertainty quantification
* 🛰️ Real-time prediction using IoT streaming data
* 📡 Deploy as a REST API or web dashboard
* 🤖 Integrate with **Reinforcement Learning** for adaptive pollution control strategies

---

## 🤝 Contributing

Contributions are welcome! 🎉

1. Fork the repo
2. Create a new branch (`feature-xyz`)
3. Commit changes
4. Open a Pull Request

Please follow [CONTRIBUTING.md](CONTRIBUTING.md) (if added) for guidelines.

---
