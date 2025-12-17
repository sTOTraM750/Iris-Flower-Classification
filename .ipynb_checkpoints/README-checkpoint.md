Project Overview:

# Iris Flower Classification using Machine Learning

This project builds a complete machine learning pipeline to classify Iris flower species
based on morphological features such as sepal length, sepal width, petal length, and petal width.

The focus of this project is not only on model accuracy, but also on understanding
data patterns, model behavior, and evaluation in a clear and structured way.

---

## Problem Overview

- **Input:** Sepal length, sepal width, petal length, petal width  
- **Output:** Iris species (Setosa, Versicolor, Virginica)  
- **Task Type:** Multiclass classification  

---

## Dataset

- Total samples: 150  
- Classes: 3 (balanced)  
- Features: 4 continuous numerical features  

The dataset is clean, well-structured, and commonly used to understand
classification fundamentals and data geometry.

---

## Workflow

1. Load and inspect the dataset  
2. Perform exploratory data analysis to understand feature relationships  
3. Split data into training and testing sets  
4. Apply feature scaling where required  
5. Train a baseline classification model  
6. Train advanced models to improve performance  
7. Evaluate models using accuracy and confusion matrices  
8. Visualize data structure and model behavior using 2D and 3D plots  
9. Compare models and select the best-performing one  

---

## Models Used

- Logistic Regression (baseline)
- K-Nearest Neighbors (KNN)
- Support Vector Machine (RBF kernel)
- Random Forest
- Neural Network (MLP)

---

## Model Evaluation

- Accuracy score
- Classification report
- Confusion matrix

Most misclassifications occur between **Versicolor** and **Virginica**, which
have overlapping feature regions. Setosa is consistently classified correctly.

---

## Visualizations

The project includes multiple visualizations to improve understanding:

- Feature correlation heatmap  
- 2D scatter plots for class separability  
- 3D PCA plot showing global data structure  
- 3D neural network decision surface showing probability behavior  

These visualizations help explain *why* models perform the way they do.

---

## Results Summary

Non-linear models such as **SVM (RBF)** and **Random Forest** outperform the
linear baseline by capturing curved decision boundaries in feature space.
SVM provides the best overall balance between accuracy and stability.

---

## Project Structure


iris-sage-ml/
│── README.md
│── requirements.txt
│
├── notebooks/
│ └── iris_sage_ml.ipynb
│
├── src/
│ ├── data_loader.py
│ ├── preprocessing.py
│ ├── models.py
│ ├── evaluation.py
│ └── visualization.py
│
└── results/
├── plots/
└── metrics/
