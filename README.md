# ELE489 HW2 – Decision Trees and Gini Index Analysis

This repository contains my solution for Homework 2 of ELE489: Fundamentals of Machine Learning at Hacettepe University. The assignment is divided into two parts:

1. **Manual Gini Index Computation (Q1):**  
   I manually computed the Gini index for a small dataset to determine the optimal root node for a decision tree based on two features: Weather and Wind.

2. **Decision Tree Analysis on the Banknote Authentication Dataset (Q2):**  
   I implemented a decision tree classifier using Scikit-learn on the Banknote Authentication dataset from the UCI Machine Learning Repository. The notebook includes data visualization, model training, evaluation, and analysis.

## Repository Structure

- **HW2_Report.tex**  
  LaTeX source file for the final homework report. It includes detailed manual calculations for Q1 and analysis for Q2.

- **decision_tree.ipynb**  
  A Jupyter Notebook that covers data exploration, model training, and evaluation for Q2. It includes visualizations such as pair plots, correlation heatmaps, decision tree diagrams, and feature importance plots.

- **README.md**  
  This file, which provides an overview of the project and instructions for running the code.

- **(Data Files)**  
  If applicable, a local copy of the Banknote Authentication dataset (or instructions to download it).

## Dataset Details

### Q1 – Manual Gini Calculation
- **Features:**  
  - **Weather:** {Sunny, Overcast, Rainy}  
  - **Wind:** {Weak, Strong}  
- **Target:** Whether a person will play outside (Yes/No)

### Q2 – Banknote Authentication Dataset
- **Source:** [UCI Banknote Authentication Dataset](https://archive.ics.uci.edu/dataset/267/banknote+authentication)
- **Instances:** 1372 samples  
- **Features:** 4 numerical features (variance, skewness, kurtosis, entropy)  
- **Class Labels:** 0 (fake) and 1 (authentic)

## Features and Implementation

- **Manual Gini Index Computation (Q1):**  
  I calculated the overall Gini index and the weighted Gini index for splits on both Weather and Wind. The feature with the lower weighted Gini was chosen as the root node.

- **Decision Tree Classifier (Q2):**  
  I used Scikit-learn’s `DecisionTreeClassifier` to train models on the Banknote Authentication dataset. I experimented with parameters such as `max_depth`, `min_samples_split`, and `criterion` ("gini" vs. "entropy"). The model’s performance is evaluated using accuracy, confusion matrices, and classification reports.

- **Visualizations:**  
  The notebook contains various plots:
  - **Pairwise Feature Plot:** to inspect the separation of classes.
  - **Correlation Heatmap:** to examine relationships among features.
  - **Decision Tree Visualization:** using `plot_tree()` to illustrate the structure.
  - **Feature Importance Plot:** to highlight the contribution of each feature in the decision tree.

## How to Run

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/YourUsername/YourRepoName.git
   cd YourRepoName
