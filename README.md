Spotify Songs Analysis: Predicting Musical Popularity
Executive Summary
What makes a song a hit? This project investigates the relationship between musical audio features and popularity scores using a dataset of 32,000+ Spotify tracks. By rigorously evaluating four different machine learning models, the analysis seeks to quantify which sonic ingredients matter most and how different model architectures (from linear models to neural networks) handle the nuances of musical data.

Objectives
Feature Mapping: Quantify how audio characteristics like energy and danceability connect to popularity.

Model Benchmarking: Compare the performance and interpretability of Linear Regression, Random Forest, XGBoost, and Neural Networks (MLP).

Error Diagnosis: Analyze residual patterns to identify systematic model biases.

Genre Analysis: Investigate how popularity distributions vary across musical categories.

Stress-Testing: Validate model predictions using hypothetical, synthetic tracks.

Tech Stack
Language: Python

Data Manipulation: Pandas, NumPy

Machine Learning: Scikit-learn, XGBoost

Visualization: Plotly (Interactive 3D scatter plots and heatmaps), Matplotlib

Methodology
1. Data Preparation & Cleaning
The raw dataset was cleaned using mean imputation for missing numeric values and mode imputation for categorical data. The data was also sorted chronologically by album release date to preserve temporal context.

2. Exploratory Data Analysis (EDA)
Correlation Heatmaps: Used to identify multicollinearity (e.g., the strong relationship between energy and loudness) and potential popularity drivers.

3D Feature Exploration: Interactive visualizations mapping energy, danceability, and loudness against popularity to find clusters of "hit" characteristics.

Genre Distributions: Baselines were established to understand which genres dominate the mainstream.

3. Predictive Modeling
The project evaluates models on a transparency–performance spectrum:

Linear Regression: For baseline interpretability.

Ensemble Methods (Random Forest/XGBoost): For capturing non-linear relationships.

Neural Networks (MLP): For complex pattern recognition.
Models are validated using 5-fold cross-validation to ensure generalizability.

Key Insights
Popularity is often driven by non-linear combinations of features rather than single characteristics.

The trade-off between model accuracy and interpretability is a core focus, guiding which models are best for "black-box" prediction versus stakeholder insights.
