# Assignment 2: Dimensionality Reduction via PCA & FDA

### Overview
This project explores the impact of dimensionality reduction on classification performance for MNIST digits (0, 1, and 2). It focuses on finding optimal feature spaces that maximize class separation while minimizing noise and redundancy.

### Technical Implementation
* **Data Preprocessing:** Images were flattened into 784-dimensional vectors and normalized to [0, 1].
* **Principal Component Analysis (PCA):** Implemented to reduce dimensions while retaining specific variance thresholds (75% and 90%).
* **Fisher's Discriminant Analysis (FDA):** Implemented to find a projection matrix that maximizes between-class variance and minimizes within-class variance.
* **Classification:** LDA and QDA models were trained on the reduced feature spaces obtained from both PCA and FDA.
* **Reconstruction Analysis:** Computed Mean Squared Error (MSE) for images reconstructed from lower-dimensional principal components.

### Results (Test Accuracy)

| Dimensionality Reduction Method | LDA Accuracy | QDA Accuracy |
| :--- | :--- | :--- |
| **PCA (75% Variance)** | **97.67%** | **96.00%** |
| **PCA (90% Variance)** | **96.67%** | **94.00%** |
| **PCA (2 Components)** | **93.33%** | **92.67%** |
| **FDA (2 Components)** | **95.67%** | **95.67%** |

### Key Observations
* **Variance vs. Noise:** Retaining 75% variance provided better test accuracy than 90%, as the latter captured more noise and led to slight overfitting.
* **FDA vs. PCA:** In 2D space, FDA achieved significantly better separation than PCA because it explicitly utilizes class labels to maximize discriminative information.
