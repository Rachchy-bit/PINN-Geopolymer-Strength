# Physics-Informed Machine Learning for Geopolymer Strength Prediction

This repository documents a research-driven approach to predicting the compressive strength of geopolymer concrete. The project demonstrates a clear progression from traditional statistical regressions and standard Deep Learning to a high-performance **Physics-Informed Neural Network (PINN)** architecture.

## 🎯 Research Objective
To overcome the limitations of standard "black-box" machine learning by integrating material science physics into the model training process, specifically focusing on the non-linear relationship between geopolymer precursors and final strength.

---

## 📊 Performance Benchmarks
A systematic evaluation was conducted to track the improvement in predictive accuracy ($R^2$) across different model architectures.

| Model Category | Algorithm | RMSE | **R² Score** | Observations |
| :--- | :--- | :--- | :--- | :--- |
| **Statistical** | Linear Regression | 0.38 | 0.467 | Failed to capture non-linear mechanics |
| **Statistical** | Lasso Regression | 0.38 | 0.461 | Similar performance to Linear |
| **Statistical** | Ridge Regression | 0.38 | 0.466 | No significant improvement |
| **Ensemble ML** | Random Forest | 0.25 | 0.772 | Significant leap; captured data patterns |
| **Deep Learning** | **ANN (Multilayer)**| **--** | **0.8866** | **Strong predictive power via Deep Learning** |
| **Physics-Informed**| **PINN** | **--** | **0.9400** | **SOTA; respects physical constraints** |

---

## 💡 Key Insight: The Value of Physics
While the **ANN (0.8866)** showed that Deep Learning can handle the data better than Random Forest, the **PINN (0.94)** proved that informing the model with material physics provides the ultimate edge. This final leap of ~5% in accuracy is critical for high-stakes structural engineering applications where precision is non-negotiable.

---

## 📂 Project Structure
- `data/`: Publicly sourced geopolymer dataset.
- `Notebook/`:
    - `geo_basic.ipynb`: Linear, Lasso, Ridge, and Random Forest baselines.
    - `geo_ann.ipynb`: Artificial Neural Network (ANN) implementation.
    - `geo_pinn.ipynb`: Physics-Informed Neural Network using the DeepXDE framework.

---

## 🛠️ Tech Stack
- **Languages:** Python
- **Core Libraries:** Pandas, NumPy, Scikit-learn
- **ML Frameworks:** TensorFlow

## 🚀 Future Work
- Expanding the PINN framework to predict durability and carbonation depth.
- Integrating these models into BIM (Building Information Modeling) workflows.

---
*Developed as an independent research project  to bridge the gap between AI and Structural Engineering.*
