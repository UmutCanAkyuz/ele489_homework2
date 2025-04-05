# ELE489 HW2 – Decision Trees and Gini Index Analysis

This repository contains my solution for Homework 2 of ELE489: Fundamentals of Machine Learning at Hacettepe University. 


**Decision Tree Analysis on the Banknote Authentication Dataset:**  
   I implemented a decision tree classifier using Scikit-learn on the Banknote Authentication dataset from the UCI Machine Learning Repository. The notebook includes data visualization, model training, evaluation, and analysis.

## Repository Structure

- **decision_tree.ipynb**  
  A Jupyter Notebook that covers data exploration, model training, and evaluation for Q2. It includes visualizations such as pair plots, correlation heatmaps, decision tree diagrams, and feature importance plots.

- **README.md**  
  This file, which provides an overview of the project and instructions for running the code.

## Dataset Details

### – Manual Gini Calculation
- **Features:**  
  - **Weather:** {Sunny, Overcast, Rainy}  
  - **Wind:** {Weak, Strong}  
- **Target:** Whether a person will play outside (Yes/No)

### – Banknote Authentication Dataset
- **Source:** [UCI Banknote Authentication Dataset](https://archive.ics.uci.edu/dataset/267/banknote+authentication)
- **Instances:** 1372 samples  
- **Features:** 4 numerical features (variance, skewness, kurtosis, entropy)  
- **Class Labels:** 0 (fake) and 1 (authentic)

## Features and Implementation

- **Decision Tree Classifier :**  
  I used Scikit-learn’s `DecisionTreeClassifier` to train models on the Banknote Authentication dataset. I experimented with parameters such as `max_depth`, `min_samples_split`, and `criterion` ("gini" vs. "entropy"). The model’s performance is evaluated using accuracy, confusion matrices, and classification reports.

- **Visualizations:**  
  The notebook contains various plots:
  - **Pairwise Feature Plot:** to inspect the separation of classes.
  - **Correlation Heatmap:** to examine relationships among features.
  - **Decision Tree Visualization:** using `plot_tree()` to illustrate the structure.
  - **Feature Importance Plot:** to highlight the contribution of each feature in the decision tree.

