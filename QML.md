# 🤖🧠 Introduction to Quantum Machine Learning (QML)

This project provides a beginner-friendly implementation of Quantum Machine Learning (QML) using **Qiskit**. It introduces the theory behind quantum data encoding, feature mapping, and classification, while implementing a **Variational Quantum Classifier (VQC)** to classify a simple dataset.

---

## 🧠 What is Quantum Machine Learning?

**Quantum Machine Learning** leverages quantum computing to enhance machine learning tasks such as classification, clustering, and regression. It integrates principles of quantum mechanics (superposition, entanglement, interference) with classical data-driven models.

QML promises potential exponential speedups and smaller model sizes for certain learning tasks. Although current hardware is limited (NISQ era), hybrid algorithms like **VQC** can already be tested using simulators.

---

##  What This Project Covers

This notebook walks through:

-  **Classical Dataset Generation:** Creating synthetic binary classification data using `make_classification`.
-  **Quantum Feature Encoding:** Encoding classical data into quantum states using angle-based rotation encoding.
-  **Variational Quantum Circuit (Ansatz):** Constructing a parameterized quantum circuit.
-  **Training with Classical Optimizer:** Using 'COBYLA' to minimize the loss between predicted and true labels.
-  **Result Evaluation:** Plotting decision boundaries.

---

##  Structure of the Notebook

1. Data Generation
2. Visualization (2D feature space)
3. Quantum Feature Map and Ansatz (Parameterized Circuit)
4. Quantum Instance Setup (QASM simulator)
5. Decision boundary

📊 Results
🔵 The dataset consists of two concentric circular classes, which are not linearly separable in their native 2D space.

📈 By applying a quantum feature map, the data is embedded into a higher-dimensional Hilbert space, making it separable with a hyperplane.

🧠 The Variational Quantum Classifier (VQC) successfully learns a non-linear decision boundary in 2D that reflects a linear separation in the quantum space.

✅ The resulting decision boundary closely matches the true class distribution, yielding classification accuracy of ~85–90%, depending on the seed and optimizer settings.

📸 Visualizations: 

The first image shows the original circular dataset.

The second image shows:

(Left) The data projected into 3D where a separating hyperplane is visible.

(Right) The 2D projection with the quantum decision boundary drawn as a black contour line.

