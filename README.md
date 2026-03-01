Hybrid VAE-WGAN-GP: Synthetic Data Augmentation for Heart Disease Prediction
📌 Project Overview
This project addresses the critical issue of data scarcity in medical datasets, specifically for Coronary Heart Disease (CHD). We propose a Hybrid VAE-WGAN-GP architecture that combines the structured latent space understanding of Variational Autoencoders (VAE) with the high-fidelity generation and training stability of Wasserstein GANs with Gradient Penalty (WGAN-GP).

By generating high-quality synthetic clinical data, we significantly improve the performance and generalizability of predictive machine learning models.

🚀 Key Results
Random Forest Accuracy: Increased from 87.25% to 92.95% using augmented data.

SVM Accuracy: Increased from 85.23% to 92.28%.

CatBoost Accuracy: Improved to 90.94%.

Optimization: Integrated Grey Wolf Optimization (GWO) for hyperparameter tuning.

🛠️ Architecture & Methodology
The pipeline consists of three distinct phases:

VAE Foundational Training: Pre-training a VAE to capture the underlying distribution and feature correlations of the tabular medical data.

WGAN-GP Refinement: Using the pre-trained VAE decoder as the foundation for the WGAN generator to refine data quality and prevent mode collapse.

Data Synthesis & Augmentation: Generating synthetic samples to achieve a 1:1 ratio with real data, followed by training ensemble classifiers.

📊 Dataset
The model was trained on a comprehensive combined dataset (including Cleveland, Hungarian, etc.) featuring:

Instances: 1190

Features: 11 clinical attributes

Target: Binary classification (Heart Disease Presence)

💻 Tech Stack
Language: Python

Deep Learning: PyTorch / TensorFlow (VAE & WGAN-GP implementation)

Machine Learning: Scikit-learn, CatBoost, XGBoost

Optimization: Grey Wolf Optimization (GWO)

Data Analysis: Pandas, NumPy, Matplotlib, Seaborn

For more details visit our website: https://ridhi-kul.github.io/Hybrid_VAE_WGANGP/