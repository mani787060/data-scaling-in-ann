# 📊 Data Scaling in Artificial Neural Networks (ANN)

## 📌 Project Overview

This project demonstrates the importance of **feature scaling when training Artificial Neural Networks (ANNs)**.

Using the **Social Network Ads** dataset, the notebook explores how features with different numerical ranges can affect neural network training, gradient descent, weight updates, and convergence.

The project compares data before and after scaling to understand why preprocessing is an essential step in Machine Learning and Deep Learning workflows.

---

## 🎯 Objective

The main objectives of this project are to:

* Understand why feature scaling is important for ANNs
* Compare data before and after scaling
* Understand the effect of feature magnitude on gradient descent
* Improve training stability and convergence
* Learn how Standardization and Min-Max Scaling work
* Build a strong foundation for preprocessing in Deep Learning

---

## 📊 Dataset

The project uses the **Social Network Ads** dataset.

The dataset contains information about users and whether they purchased a product after seeing an advertisement on a social network.

### Features Used

* **Age**
* **Estimated Salary**

### Target Variable

* **Purchased**

The target represents whether the user purchased the product.

---

## ❓ Why is Scaling Important?

Consider two features:

```text
Age              → 18 to 60
Estimated Salary → 15,000 to 150,000
```

The salary values are much larger than the age values.

Without scaling, the feature with the larger numerical range can have a disproportionate influence during optimization.

For neural networks, this can lead to:

* Uneven weight updates
* Slower convergence
* Unstable optimization
* Difficulty finding an optimal solution

Scaling puts features on comparable ranges and helps gradient-based optimization work more efficiently.

---

## 🔵 Standardization

Standardization transforms the data so that the feature generally has:

* Mean ≈ 0
* Standard deviation ≈ 1

It is commonly performed using **StandardScaler** from Scikit-learn.

```text
Original Data
      ↓
StandardScaler
      ↓
Scaled Data
```

---

## 🟠 Min-Max Scaling

Min-Max Scaling transforms values into a fixed range, commonly:

```text
0 → 1
```

This can be useful when a model benefits from features having a bounded range.

Scikit-learn provides **MinMaxScaler** for this purpose.

---

## 🔬 Project Workflow

The notebook follows the following workflow:

1. Load the Social Network Ads dataset
2. Explore the dataset
3. Select relevant features
4. Separate input features and target variable
5. Split data into training and testing sets
6. Visualize the original features
7. Apply feature scaling
8. Visualize the scaled features
9. Understand the effect of scaling on ANN training
10. Analyze the importance of preprocessing

---

## 📈 Before vs After Scaling

The notebook uses visualization to understand how scaling changes the numerical representation of the features.

### Before Scaling

Features may have significantly different ranges.

### After Scaling

Features are brought into comparable numerical ranges, making them more suitable for gradient-based optimization.

---

## 🧠 Key Concepts Covered

* Feature Scaling
* Standardization
* Min-Max Scaling
* Artificial Neural Networks
* Gradient Descent
* Weight Updates
* Model Convergence
* Data Preprocessing
* Training Stability
* Feature Distributions

---

## 🔑 Key Learnings

### 1. Feature Scale Matters

Features with very different magnitudes can negatively affect optimization algorithms.

### 2. Scaling Helps Gradient Descent

Properly scaled features generally allow gradient-based algorithms to converge more efficiently.

### 3. Scaling Is Important in Neural Networks

ANNs rely heavily on gradient-based optimization, making appropriate preprocessing especially important.

### 4. Visualization Helps

Scatter plots provide an intuitive way to understand how scaling changes feature ranges and distributions.

---

## 🛠️ Technologies Used

* **Python**
* **NumPy**
* **Pandas**
* **Matplotlib**
* **Seaborn**
* **Scikit-learn**
* **Jupyter Notebook**

---

## 📚 Learning Outcomes

After completing this project, I gained a better understanding of:

* Why feature scaling is required for many ML and DL algorithms
* How StandardScaler works
* How MinMaxScaler works
* How feature magnitude affects gradient descent
* Why preprocessing can influence model convergence
* The role of scaling in Artificial Neural Networks

---

## 🚀 Future Improvements

Possible extensions of this project include:

* Train an ANN before and after scaling
* Compare training loss and accuracy
* Visualize gradient descent convergence
* Experiment with different scaling techniques
* Compare StandardScaler, MinMaxScaler, and RobustScaler
* Analyze the effect of scaling on different neural network architectures

---

## 💡 Final Takeaway

**Data scaling is not just a preprocessing step—it can directly affect how efficiently a neural network learns.**

When features have very different ranges, scaling them to comparable ranges can help gradient-based optimization become more stable and efficient.

This project provides a practical foundation for understanding why **feature preprocessing is an important part of Machine Learning and Deep Learning workflows**.
