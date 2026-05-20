<div align="center">

# <span style="color:#3b82f6">Supervised Fish Weight Estimation (Linear Regression)</span>

![Python](https://img.shields.io/badge/Python-3.10%2B-1e293b?style=for-the-badge&logo=python&logoColor=white)
![Scikit-Learn](https://img.shields.io/badge/Scikit_Learn-Machine_Learning-f7931e?style=for-the-badge&logo=scikit-learn&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-Dataframe-150458?style=for-the-badge&logo=pandas&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-Visualization-11557c?style=for-the-badge)
![License](https://img.shields.io/badge/License-MIT-059669?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Active-3b82f6?style=for-the-badge)

<br/>

<h3>
  <em>"Predicting Continuous Biological Target Vectors via Ordinary Least Squares and Morphometric Feature Projections"</em><br/>
</h3>

<br/>

[📌 Overview](#-overview) • [✨ Features](#-features) • [🚀 Pipeline Flow](#-pipeline-flow) • [⚙️ Installation](#%EF%B8%8F-installation) • [🧠 Mathematical Foundations](#-mathematical-foundations) • [🤝 Contributing](#-contributing)

</div>

---

## 📌 Overview

**Supervised Fish Weight Estimation** is a predictive machine learning pipeline that implements **Ordinary Least Squares (OLS) Linear Regression** to model the continuous biophysical relationship between a fish's physical dimensions (*Length*) and its total structural mass (*Weight*). Utilizing biological metrics from the classic *Fish Dataset*, this repository establishes a continuous trend line to automate specimen scaling evaluations.

The architecture vectorizes input feature columns, fits structural weights to determine the growth slope coefficient, handles custom real-time inference checks ($30\text{ cm}$), and maps the global distribution alongside the prediction marker on a clear 2D Matplotlib dashboard.

---

## ✨ Features

### 🎯 Core Capabilities
| Feature | Description |
|---|---|
| 📐 **Biophysical Matrix Extraction** | Parses continuous fish measurements into structural feature arrays using Pandas. |
| 📈 **Ordinary Least Squares Fit** | Optimizes line weights by minimizing distance variations across all data points. |
| 🔮 **Target Weight Inference** | Evaluates new unseen length values ($30\text{ cm}$) to predict real-time weight scales. |
| 🎨 **Morphometric Scatter Dashboard**| Generates high-fidelity plots mapping raw indices alongside the model's regression line. |
| 🌓 **Alpha Transparency Blending** | Applies subtle element masking (`alpha=0.5`) to make high-density data overlaps easily scannable. |

### 🌟 Design Highlights
- 🧠 **Supervised Regression Blueprint** — Infers exact physical growth trend slopes from raw historical training examples ($X \rightarrow y$).
- ⚡ **Lightweight Vector Mechanics** — Built on top of Scikit-Learn's optimized linear algebra systems for instant inference calculation.
- 📉 **Continuous Prediction Outputs** — Generates precise, non-discrete target numbers ($g$), ideal for automated biological tracking.

---

## 🚀 Pipeline Flow

┌─────────────────────────────────────────────────────────┐│                    FISH BIOMETRIC DATASET INGESTION     ││       (Features: Length1 Matrix Indices | Target: Weight)│└─────────────────────────────────────────────────────────┘│▼[ Feature Array Vectorization & Reshaping (X, y) ]│▼┌───────────────────────────────────────────────────────┐│               LINEAR REGRESSION FITTING               ││     Compute Residual Variances ──► Extract Growth Slope │└───────────────────────────┬───────────────────────────┘│▼[ Establish Continuous Weight Trend Boundary Line ]│▼┌───────────────────────────────────────────────────────┐│               TARGET INFERENCE TESTING                ││   Evaluate 30cm Fish Sample via Trained Coefficients  │└───────────────────────────┬───────────────────────────┘│▼┌─────────────────────────────────────────────────────────┐│                 BIOMETRIC VISUALIZATION DASHBOARD       ││                                                         ││   Render: Matplotlib 2D Coordinate Scatter Grid         ││   Line: Sloped regression line tracking actual growth   ││   Marker: Custom 'X' point highlighting the prediction  │└─────────────────────────────────────────────────────────┘
---

## ⚙️ Installation

### Prerequisites

Make sure your local computer has these foundational software components set up:
- Python 3.10+
- Git

---

### 🔧 Step-by-Step Setup

**1. Clone the Repository**
```bash
git clone [https://github.com/jaweriashakoor/Supervised-Fish-Weight-LinearRegression.git](https://github.com/jaweriashakoor/Supervised-Fish-Weight-LinearRegression.git)
cd Supervised-Fish-Weight-LinearRegression
2. Create a Virtual EnvironmentBashpython -m venv myenv

# Windows (PowerShell)
.\myenv\Scripts\Activate.ps1

# Linux / macOS
source myenv/bin/activate
3. Install DependenciesBashpip install numpy pandas scikit-learn matplotlib
4. Execute the Estimation ScriptBashpython fish_weight_regression.py
🧠 Mathematical FoundationsThe Morphometric Prediction FormulaThe model estimates the growth trajectory of a specimen using a single-variable linear regression equation:$$y = \beta_0 + \beta_1 x + \epsilon$$Where:$y$ represents the continuous predicted weight target value (in grams).$x$ represents the recorded feature length measurement (in centimeters).$\beta_1$ represents the regression coefficient (the slope defining weight increase per centimeter).$\beta_0$ represents the y-intercept baseline value.$\epsilon$ represents the structural error residual.The Objective Minimization CostTo construct the trend line, the algorithm minimizes the Residual Sum of Squares (RSS) across the dataset:$$RSS = \sum_{i=1}^{n} (y_i - \hat{y}_i)^2$$Where $y_i$ is the actual recorded fish weight and $\hat{y}_i$ is the value estimated by the trend boundary. Finding the exact spot where the cost derivative drops to zero ensures optimal prediction accuracy for custom inputs.🤝 ContributingContributions help keep our open-source tools robust, optimized, and ready for development!Bash# 1. Fork the Project Repository
# 2. Setup your feature branch
git checkout -b feature/polynomial-growth-mapping

# 3. Commit functional updates
git commit -m "Add: Implement polynomial feature transformations to capture non-linear growth curves"

# 4. Push updates to origin branch
git push origin feature/polynomial-growth-mapping

# 5. Open a Pull Request
📄 LicenseThis analysis pipeline is distributed as open-source software under the terms of the MIT License.
