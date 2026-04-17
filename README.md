# Statistical Machine Learning

### Overview
This repository contains a collection of from-scratch implementations of fundamental statistical machine learning algorithms. The focus of these projects is on probabilistic modeling, dimensionality reduction, and mathematical derivations for classification and regression, rather than relying on high-level black-box abstractions. 

All models are built, trained, and tested on the MNIST and Fashion MNIST datasets to evaluate their performance, feature space separation and predictive accuracy.

### Technologies Used
* **Language:** Python
* **Core Libraries:** NumPy, Pandas
* **Visualization:** Matplotlib, scikit-learn (strictly for t-SNE projections and Lasso)
* **Documentation:** LaTeX

---

### Repository Structure

#### [Assignment 1: MLE & Discriminant Analysis](./Assignment-1-MLE-Discriminant-Analysis)
* **Topics:** Maximum Likelihood Estimation (MLE), Linear Discriminant Analysis (LDA), Quadratic Discriminant Analysis (QDA).
* **Summary:** Modeled multivariate Gaussian distributions for MNIST digits and implemented linear and quadratic discriminant functions to classify test samples, achieving up to 99% accuracy.

#### [Assignment 2: Dimensionality Reduction (PCA & FDA)](./Assignment-2-PCA-FDA)
* **Topics:** Principal Component Analysis (PCA), Fisher's Discriminant Analysis (FDA), Eigenvalue Decomposition.
* **Summary:** Implemented dimensionality reduction pipelines to optimize feature spaces. Compared variance retention strategies (75% vs 90%) and analyzed the differences between unsupervised (PCA) and supervised (FDA) projection techniques.

#### [Assignment 3: Regularization & Ensembles](./Assignment-3-Regularization-and-Ensembles)
* **Topics:** Ridge & Lasso Regression, Decision Trees, Bagging, Random Forests, Out-of-Bag (OOB) Error.
* **Summary:** Implemented regularized linear models to analyze feature sparsity and built custom decision trees using the weighted Gini index and Sum of Squared Residuals (SSR). Extended base trees into Bagged and Random Forest ensembles to demonstrate variance reduction on the MNIST and Fashion MNIST datasets.
