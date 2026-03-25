# 🚀 Deep Learning Lab Projects 

This repository contains **three deep learning projects implemented in a single Jupyter Notebook** using PyTorch.

The projects focus on:

* CNN (Convolutional Neural Networks)
* LSTM (Long Short-Term Memory)
* Model optimization and performance improvement

---

## 📂 Project Structure

```
QUEST_Lab_Project.ipynb   # Contains all 3 projects
README.md
```

---

## 📌 Projects Overview

### 1️⃣ CNN Image Classification (Synthetic Data)

* Built a Convolutional Neural Network using PyTorch
* Used **FakeData dataset (randomly generated images)**

**Demonstrations:**

* Model training on synthetic data
* Overfitting behavior
* Effect of batch size
* Regularization using Dropout and Weight Decay

**Key Learning:**
Since the dataset is random, the model cannot learn meaningful patterns, resulting in accuracy around **10% (random guess)**.

---

### 2️⃣ NLP Sentiment Analysis using LSTM

* Implemented an LSTM model for text classification
* Used a **messy synthetic dataset with missing values (NaNs)**

**Steps Covered:**

* Handling missing values in text and labels
* Feature engineering (text length)
* Training LSTM model
* Evaluating performance before and after cleaning

---

### 3️⃣ Model Optimization & Training Speed Improvement

* Built a regression model using a simple neural network
* Used a **synthetic dataset**

**Before Optimization:**

* Very small batch size (1)
* Used SGD optimizer
* Training was slow

**After Optimization:**

* Increased batch size (32)
* Switched to Adam optimizer
* Faster convergence and reduced training time

**Key Learning:**

* Batch size significantly affects training speed
* Adam optimizer converges faster than SGD
* Efficient training improves performance and time

---

## ⚙️ Installation

Make sure Python 3.8+ is installed.

Install required libraries:

```bash
pip install torch torchvision pandas numpy scikit-learn matplotlib
```

---

## 💻 How to Run

1. Clone the repository:

```bash
git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name
```

2. Open Jupyter Notebook:

```bash
jupyter notebook
```

3. Run:

```
QUEST_Lab_Project.ipynb
```

---

## 🖥️ Device Support

The code automatically detects GPU:

```python
device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
```

---

## 📊 Results Summary

| Project                | Result                                   |
| ---------------------- | ---------------------------------------- |
| CNN (FakeData)         | ~10% accuracy (random data)              |
| LSTM (Before Cleaning) | Unstable performance                     |
| LSTM (After Cleaning)  | Improved accuracy                        |
| Optimization Project   | Faster training with Adam & larger batch |

---

## 🧠 Learning Outcomes

* Understanding deep learning workflows
* Building CNN and LSTM models
* Handling missing and noisy data
* Improving model performance using preprocessing
* Optimizing training speed and efficiency

---

## 🚀 Future Improvements

* Use real datasets for better learning
* Add training graphs (loss/accuracy)
* Implement advanced models

---


## ⭐ Acknowledgements

* PyTorch Documentation
* Open-source ML community

---
