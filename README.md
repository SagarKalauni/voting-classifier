<div align="center">

# 🦁 Voting Classifier (Hard vs. Soft Voting) — Interactive Masterclass
### **Lindenwood University — Interactive Data Science & Machine Learning Masterclass**

[![Live Interactive Lab](https://img.shields.io/badge/Launch_Interactive_Lab-Live_Demo-C5B358?style=for-the-badge&logo=googlechrome&logoColor=black)](https://sagarkalauni.github.io/voting-classifier/)
[![Course](https://img.shields.io/badge/Course-DSCI_35600-000000?style=for-the-badge&logo=academia&logoColor=C5B358)](#)
[![Author](https://img.shields.io/badge/Faculty-Sagar_Kalauni,_M.S.-1E293B?style=for-the-badge&logo=github&logoColor=white)](https://github.com/SagarKalauni)

</div>

---

## 📖 Overview

An interactive demonstration of **Heterogeneous Ensemble Learning (Voting Classifiers)**. Students compare how diverse base estimators (e.g., Logistic Regression, SVM, KNN, Decision Trees) combine predictions through **Hard (Majority) Voting** versus **Soft (Probability-Averaged) Voting**.

> 🔗 **Launch the Live Interactive Application:** [**https://sagarkalauni.github.io/voting-classifier/**](https://sagarkalauni.github.io/voting-classifier/)

---

### 📐 Mathematical Formulation

Let ${C_1, C_2, \dots, C_M}$ be $M$ distinct base classifiers trained on dataset $\mathcal{D}$.

1. **Hard Voting (Majority Rule):** Predicts the class label that receives the highest number of discrete votes:
   $$\hat{y}_{\text{hard}}(\mathbf{x}) = \underset{k \in \{1, \dots, K\}}{\arg\max} \sum_{m=1}^{M} w_m \, \mathbb{I}\!\left(C_m(\mathbf{x}) = k\right)$$
2. **Soft Voting (Weighted Probability Calibration):** Averages the predicted class membership probabilities $\hat{P}_m(y = k \mid \mathbf{x})$ across all estimators:
   $$\hat{y}_{\text{soft}}(\mathbf{x}) = \underset{k \in \{1, \dots, K\}}{\arg\max} \frac{1}{\sum_{j=1}^M w_j} \sum_{m=1}^{M} w_m \, \hat{P}_m(y = k \mid \mathbf{x})$$

---

## ✨ Key Interactive Features

- **Hard vs. Soft Voting Comparison:** Toggle between discrete ballot counting and calibrated probability averaging.
- **Heterogeneous Base Learners:** Compare linear, kernel, and instance-based models side by side.
- **Custom Estimator Weights:** Adjust classifier confidence weights $w_m$ and observe immediate shifts in the ensemble decision boundary.
- **Condorcet's Jury Theorem Intuition:** Demonstrate how combining independent weak learners surpasses the accuracy of any single model.

---

## 🎓 Pedagogical & Course Context

- **Institution:** Lindenwood University (*College of Science, Technology, and Health*)
- **Course Curriculum:** DSCI 35600 — Machine Learning
- **Instructor & Author:** **Sagar Kalauni, M.S.** (*Full-Time Faculty in Data Science*)
- **Tech Stack:** HTML5, Tailwind CSS, **D3.js** (Dynamic Data Visualization), **MathJax** (LaTeX Mathematical Rendering), Vanilla ES6+ JavaScript (Zero-Dependency Client-Side Execution).

---

## 🚀 Running Locally

Because this visualizer is engineered as a self-contained, zero-build client-side application, you can run it immediately in any modern browser:

```bash
# Clone the repository
git clone https://github.com/SagarKalauni/voting-classifier.git

# Navigate into the project directory
cd voting-classifier

# Open index.html directly in your browser or serve locally:
python -m http.server 8000
```

---

## 🔗 Explore the Complete Interactive Masterclass Suite

| Module | Topic | Live Link |
| :--- | :--- | :---: |
| **Linear Regression** | Ordinary Least Squares & Residual Minimization | [Launch](https://sagarkalauni.github.io/linear-regression/) |
| **Logistic Regression** | Sigmoid Probabilities & Binary Cross-Entropy | [Launch](https://sagarkalauni.github.io/logistic-regression/) |
| **Regularization ($L_1 / L_2$)** | Lasso vs. Ridge Constraint Geometry | [Launch](https://sagarkalauni.github.io/Regularization/) |
| **K-Nearest Neighbors** | Instance-Based Learning & Distance Metrics | [Launch](https://sagarkalauni.github.io/knn/) |
| **Support Vector Machine** | Maximum-Margin Hyperplanes & Soft Margin $C$ | [Launch](https://sagarkalauni.github.io/support-vector-machine/) |
| **RBF Kernel SVM** | Non-Linear Kernel Trick & $(\gamma, C)$ Tuning | [Launch](https://sagarkalauni.github.io/rbf-kernel-svm/) |
| **Decision Tree (CART)** | Recursive Splitting, Gini & Entropy | [Launch](https://sagarkalauni.github.io/decision-tree/) |
| **Random Forest** | Bagging & Ensemble Variance Reduction | [Launch](https://sagarkalauni.github.io/random-forest/) |
| **Voting Classifier** | Hard Majority vs. Soft Probability Voting | [Launch](https://sagarkalauni.github.io/voting-classifier/) |
| **K-Means Clustering** | Lloyd's Algorithm, Voronoi & Elbow WCSS | [Launch](https://sagarkalauni.github.io/k-mean-clustering/) |
| **Confusion Matrix** | Precision, Recall, Specificity & $F_1$-Score | [Launch](https://sagarkalauni.github.io/confusion-matrix/) |
| **Confidence vs. Prediction Intervals** | Mean Response vs. Individual Uncertainty | [Launch](https://sagarkalauni.github.io/confidence-and-prediction-interval/) |
| **Bootstrapping** | Non-Parametric Resampling with Replacement | [Launch](https://sagarkalauni.github.io/bootstrap/) |
| **Q-Q Plot** | Gaussian Normality & Tail Diagnostics | [Launch](https://sagarkalauni.github.io/qq-plot/) |
| **Train-Test Split & CV** | Holdout Partitioning & $K$-Fold Cross-Validation | [Launch](https://sagarkalauni.github.io/split/) |
| **One-Hot Encoding** | Categorical Expansion & Dummy Variable Trap | [Launch](https://sagarkalauni.github.io/one-hot-encoding/) |

---

<div align="center">
  <sub>Developed with ❤️ for Data Science students by <a href="https://github.com/SagarKalauni">Sagar Kalauni</a> · <a href="https://sagarkalauni.github.io">Portfolio</a></sub>
</div>
