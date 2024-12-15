Music Genre Classification Using Machine Learning

Welcome to the repository for the Music Genre Classification project! This project explores the use of machine learning techniques to predict music genres based on audio features. It was developed as part of the DATA1030 course at Brown University.

Overview

Music is a vital part of human culture, shaping identities and enabling innovation in various interactive applications such as music recommendation systems, playlist generation, and audio analysis. This project aims to classify music tracks into one of 11 genres using audio features. The dataset was sourced from Kaggle and Machine Hack.

Key Features
	•	Comprehensive Exploratory Data Analysis: Visualizations to uncover trends, correlations, and challenges such as data imbalance and missing values.
	•	Preprocessing Pipeline: Handles missing values, scales features, and ensures balanced splits for training and testing.
	•	Implementation of six Machine Learning Models:
		•	Logistic Regression (L2 and ElasticNet)
		•	Random Forest
		•	Support Vector Classifier (SVC)
		•	XGBoost
		•	K-Nearest Neighbors
	•	Evaluation Metrics:
		•	Log Loss as the primary metric, capturing model confidence across class probabilities.
		•	Macro F1 as a side reference for class imbalance evaluation.

Repository Structure
.
├── data/               # Contains the dataset used for training and evaluation
├── figures/            # Visualization outputs (e.g., plots, confusion matrices)
├── results/            # Model evaluation results and logs
├── notebooks/          # Jupyter notebooks with EDA, preprocessing, and modeling
├── src/                # Python scripts for pipelines and utilities
├── README.md           # This file

Results
	•Best Model: XGBoost, achieving a 31% reduction in log loss compared to the baseline and the highest Macro F1 score (0.4753).
	•Key Features: Acousticness, instrumentalness, and popularity were consistently identified as the most important predictors across feature importance analyses.

Future Directions
	•Fine-tune hyperparameters by expanding search ranges.
	•Explore oversampling techniques like SMOTE to address class imbalance.
	•Incorporate additional audio features and external data for improved genre classification.
	•Experiment with reduced-feature models for interpretability.
