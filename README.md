# 🍷 Wine Cultivar Classification using Machine Learning

<p align="center">
  <b>Explore Wine Chemistry. Analyze Data. Predict Wine Cultivars.</b>
  <br>
  A Machine Learning project focused on exploring chemical properties of wine and classifying wine cultivars using supervised learning algorithms.
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Language-Python-3776AB?style=for-the-badge&logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/ML-Scikit--learn-F7931E?style=for-the-badge&logo=scikitlearn&logoColor=white" />
  <img src="https://img.shields.io/badge/Analysis-Pandas-150458?style=for-the-badge&logo=pandas" />
  <img src="https://img.shields.io/badge/Environment-Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white" />
</p>

---

## 📌 About the Project

**Wine Cultivar Classification** is a Machine Learning project that explores the Wine Recognition Dataset available in Scikit-learn.

The dataset contains chemical analysis results of wines belonging to three different cultivars grown in Italy. The project uses these chemical properties to train supervised Machine Learning models that classify wines into their respective cultivar categories.

It demonstrates a basic end-to-end Machine Learning workflow, starting from data exploration and preprocessing to model training, feature scaling, cross-validation, hyperparameter tuning, and model evaluation.

The implementation is organized into two Jupyter Notebooks to explain the process step by step.

---

## 🎯 Project Objectives

- Understand and explore the Wine Recognition Dataset.
- Perform Exploratory Data Analysis (EDA).
- Analyze chemical properties using data visualization.
- Prepare feature and target variables.
- Implement K-Nearest Neighbors (KNN) classification.
- Implement Logistic Regression.
- Understand the importance of feature scaling.
- Apply cross-validation for model selection.
- Perform hyperparameter tuning using GridSearchCV.
- Evaluate classification performance on unseen data.
- Predict wine cultivars using new observations.

---

## 📊 Dataset Information

The project uses the built-in Wine Recognition Dataset from Scikit-learn.

| Attribute | Details |
|---|---|
| Total Samples | 178 |
| Number of Features | 13 |
| Number of Classes | 3 |
| Problem Type | Multiclass Classification |
| Feature Type | Numerical |
| Missing Values | None |

### 🧪 Chemical Features

The dataset contains the following 13 chemical attributes:

1. Alcohol
2. Malic Acid
3. Ash
4. Alcalinity of Ash
5. Magnesium
6. Total Phenols
7. Flavanoids
8. Nonflavanoid Phenols
9. Proanthocyanins
10. Color Intensity
11. Hue
12. OD280/OD315 of Diluted Wines
13. Proline

---

## 🛠️ Technology Stack

| Technology | Purpose |
|---|---|
| 🐍 Python | Core programming language |
| 🐼 Pandas | Data manipulation and analysis |
| 🔢 NumPy | Numerical operations |
| 📊 Matplotlib | Data visualization |
| 🎨 Seaborn | Statistical visualization |
| 🤖 Scikit-learn | Machine Learning algorithms and evaluation |
| 📓 Jupyter Notebook | Interactive development environment |

---

## 📂 Project Structure

```text
├── Getting_Started_to_Wine_Recognition_Dataset.ipynb
│
├── Model_Evaluation_Wine_Recognition_Dataset.ipynb
│
├── README.md
```

---

## 🔄 Project Workflow

### 1. Data Exploration and Preparation

**Notebook:** `Getting_Started_to_Wine_Recognition_Dataset.ipynb`

- Load the Wine Recognition Dataset from Scikit-learn.
- Convert the dataset into a Pandas DataFrame.
- Inspect dataset structure and data types.
- Generate descriptive statistics.
- Check missing values and duplicate records.
- Analyze wine cultivar distribution.
- Visualize chemical attributes using Seaborn pairplots.
- Separate features (X) and target (y).
- Perform stratified train-test splitting.

### 2. Model Training and Evaluation

**Notebook:** `Model_Evaluation_Wine_Recognition_Dataset.ipynb`

- Understand training accuracy and testing accuracy.
- Implement KNN classification with K = 5.
- Implement Logistic Regression.
- Experiment with KNN using K = 1.
- Apply StandardScaler for feature scaling.
- Explore different K values from 1 to 25.
- Perform five-fold cross-validation.
- Use GridSearchCV for hyperparameter tuning.
- Visualize cross-validation accuracy.
- Evaluate models using accuracy, confusion matrix, precision, recall, and F1-score.
- Predict wine cultivars using new observations.

---

## 🤖 Machine Learning Algorithms

| Algorithm / Technique | Purpose |
|---|---|
| KNN (K = 1) | Classification using the nearest neighbor |
| KNN (K = 5) | Classification using five nearest neighbors |
| Logistic Regression | Multiclass classification |
| StandardScaler | Standardization of numerical features |
| Cross-Validation | Evaluating model performance across multiple data splits |
| GridSearchCV | Finding a suitable K value through cross-validation |

---

## ⚙️ Important Machine Learning Concepts

### 1. Feature Scaling

StandardScaler is used to standardize numerical features before model training.

This is particularly important for KNN because it uses distance calculations to identify neighboring data points. Features with larger numerical ranges could otherwise dominate the distance calculation.

### 2. Cross-Validation

Five-fold cross-validation is used to evaluate different K values.

The dataset is divided into five parts, with each part being used for validation once while the remaining parts are used for training.

### 3. Hyperparameter Tuning

GridSearchCV searches through K values from 1 to 25 and identifies the value that provides the best mean cross-validation accuracy.

### 4. Model Evaluation

The selected model is evaluated on a separate testing dataset to estimate its performance on unseen observations.

Evaluation metrics include:

- Accuracy
- Confusion Matrix
- Precision
- Recall
- F1-Score

---

## 🏗️ Machine Learning Workflow

```text
       Wine Recognition Dataset
                  |
                  v
          Data Exploration
                  |
                  v
       Exploratory Data Analysis
                  |
                  v
        Feature and Target Split
                  |
                  v
        Stratified Train-Test Split
                  |
                  v
           Feature Scaling
                  |
                  v
          Model Training
                  |
          +-------+-------+
          |               |
          v               v
       KNN Model    Logistic Regression
          |
          v
    Hyperparameter Tuning
          |
          v
       GridSearchCV
          |
          v
     Model Evaluation
          |
          v
    Wine Cultivar Prediction
```

---

## 🚀 Getting Started

### Prerequisites

- Python 3.x
- Jupyter Notebook
- pip package manager

### Installation

**1. Clone the repository**

```bash
git clone https://github.com/srxxr4man/wine-cultivar-classification.git
```

**2. Navigate to the project directory**

```bash
cd Wine-Cultivar-Classification
```

**3. Launch Jupyter Notebook**

```bash
jupyter notebook
```

**4. Run the notebooks in order**

- `01_wine_data_exploration.ipynb`
- `02_wine_model_evaluation.ipynb`

Run the cells sequentially to understand the complete Machine Learning workflow.

---

## 🎓 Learning Outcomes

Through this project, I explored:

- Data loading and manipulation using Pandas.
- Exploratory Data Analysis and visualization.
- Feature extraction and target separation.
- Training and testing datasets.
- Supervised Machine Learning algorithms.
- KNN and Logistic Regression.
- Feature scaling and standardization.
- Cross-validation and hyperparameter tuning.
- Model evaluation using classification metrics.
- Prediction using trained classification models.

---

## 🔮 Future Improvements

- Compare additional classification algorithms.
- Implement Support Vector Machines and Decision Trees.
- Perform advanced hyperparameter optimization.
- Build an interactive wine cultivar prediction interface.
- Deploy the trained model as a web application.
- Develop a dashboard for visualizing chemical properties and predictions.

---

## 📚 Dataset Source

**Scikit-learn Wine Recognition Dataset**

[View Official Dataset Documentation](https://scikit-learn.org/stable/modules/generated/sklearn.datasets.load_wine.html)

---

## 🎓 Academic Details

| Detail | Information |
|---|---|
| Institution | Muthoot Institute of Technology and Science (MITS) |
| Department | Artificial Intelligence and Data Science |
| Academic Batch | 2025–2029 |
| Project Domain | Machine Learning |
| Programming Language | Python |

---

## 👨‍💻 Author

**A Sreeram**

Artificial Intelligence and Data Science Student  
Muthoot Institute of Technology and Science (MITS)

Interested in Machine Learning, Python, Data Science, and Artificial Intelligence.

---

<p align="center">
  ⭐ If you find this project useful, consider giving this repository a star!
  <br><br>
  <b>🍷 Exploring Data. Learning Machine Learning. Building Intelligence.</b>
</p>
