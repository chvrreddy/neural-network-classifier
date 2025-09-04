# Neural Network from Scratch — Classifying A/B/C (5×6 Binary Images)

## 📌 Project Overview
This project implements a **two-layer feedforward neural network** using only **NumPy** to classify small **5×6 binary images** of the characters **A, B, and C**.  
- Input: Flattened 5×6 = 30-dimensional binary vector.  
- Hidden Layer: Configurable (default = 16 neurons).  
- Output Layer: 3 neurons (one for each class).  
- Activation: **Sigmoid** (hidden and output layers).  
- Loss: **Binary Cross-Entropy (BCE)**.  
- Optimizer: **Gradient Descent** (manual backpropagation).  

The network is trained to recognize clean and noisy versions of A, B, and C.

---

## 📂 Dataset
- Each class (A, B, C) is represented as a **5×6 binary pattern**.  
- To make the dataset larger, **random noise** is applied by flipping pixels with a small probability (default 5%).  
- Labels are **one-hot encoded**:  
  - `[1,0,0]` = A  
  - `[0,1,0]` = B  
  - `[0,0,1]` = C  

---

## ⚙️ Features
- Neural network built **completely from scratch with NumPy**.  
- Manual implementation of **forward pass** and **backpropagation**.  
- Tracks and plots **loss & accuracy curves**.  
- Visualizes **clean and noisy image predictions** with `matplotlib`.  
- Easy to adjust hyperparameters (hidden size, learning rate, epochs, noise level).

---

## 🛠️ Requirements
- Python 3.x  
- NumPy  
- Matplotlib  

Install dependencies (if needed):
```bash
pip install numpy matplotlib
