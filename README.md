# PCA vs LDA on Fashion-MNIST: Dimensionality Reduction & Visualization

This project demonstrates the application of **Principal Component Analysis (PCA)** and **Linear Discriminant Analysis (LDA)** for dimensionality reduction and visualization using the **Fashion-MNIST** dataset.

---

### 🧵 Dataset Overview

Fashion-MNIST consists of **28x28 grayscale images** of 10 fashion categories:

- T-shirt/top
- Trouser
- Pullover
- Dress
- Coat
- Sandal
- Shirt
- Sneaker
- Bag
- Ankle boot

Each image is flattened to a 784-dimensional vector.

---

### 📋 Task Steps

1. **Load Dataset**
   - Load the Fashion-MNIST dataset using `keras.datasets.fashion_mnist`
   - Split into training and test sets

2. **Preprocess**
   - Normalize pixel values to [0, 1]
   - Visualize at least one image from each class using `matplotlib`

3. **Apply PCA**
   - Use `sklearn.decomposition.PCA` to reduce dimensions from 784 → 2
   - PCA is unsupervised (no class labels used)

4. **Apply LDA**
   - Use `sklearn.discriminant_analysis.LinearDiscriminantAnalysis` to reduce to 2D
   - LDA uses class labels for supervised projection

5. **Visualize Results**
   - 2D Scatter plots for both PCA and LDA
   - Each class shown in a distinct color

---

### 📊 Visual Comparison

- **PCA**: Captures maximum variance, but class clusters may overlap
- **LDA**: Maximizes class separability using label information

> 🧠 **Insight:** LDA generally shows better class separation than PCA in labeled data scenarios like classification tasks.

---

### 🧠 When to Use

| Use Case | Recommended Method |
|----------|--------------------|
| Data Exploration (No Labels) | PCA |
| Classification Tasks (With Labels) | LDA |
| Noise Reduction | PCA |
| Feature Engineering for Supervised Models | LDA |

---

### 📁 Files Included

- `Question.pdf` – Full task description
- `Solution.pdf` – Python notebook with visualizations and code

---
