# Assignment 3: Regularization, Decision Trees & Ensemble Methods

### Overview
This project focuses on implementing regularized linear models and tree-based ensemble methods from scratch. The objective was to handle classification and regression tasks on the MNIST and Fashion MNIST datasets, exploring how model complexity, feature selection, and variance reduction techniques impact performance.

### Technical Implementation
* **Regularized Regression (Q1):** Implemented **Ridge** and **Lasso** regression for classification on PCA-reduced MNIST data. Analyzed the effect of the penalty parameter ($\lambda$) on training/test Mean Squared Error (MSE) and plotted regularization paths to visualize Lasso's feature selection (sparsity) capabilities. Evaluated model complexity by varying PCA dimensions.
* **Decision Trees & Random Forests (Q2):** Built a custom Decision Tree classifier from scratch using the **weighted Gini index** to evaluate optimal splitting thresholds. Extended this into ensemble models by implementing **Bagging** and **Random Forests** (with random feature subsampling at splits). Calculated **Out-of-Bag (OOB) error** to evaluate ensemble performance without a separate validation set.
* **Regression Trees (Q3):** Transitioned to the Fashion MNIST dataset to build regression **Decision Stumps** (single-split trees). Evaluated candidate splits using the **Sum of Squared Residuals (SSR)**. Applied Bagging to the regression stumps to demonstrate variance reduction, comparing the predictive performance of a single stump versus the bagged ensemble.

### Key Observations
* **Regularization:** Demonstrated how Lasso actively shrinks less important feature coefficients to exactly zero, performing automatic feature selection, whereas Ridge shrinks them asymptotically.
* **Model Complexity:** Showed the trade-off between PCA dimensions and test MSE, highlighting the point where adding more dimensions leads to overfitting rather than better generalization.
* **Ensemble Superiority:** Quantified the performance gains of Bagging and Random Forests over single decision trees, utilizing OOB error as a reliable proxy for test accuracy.
