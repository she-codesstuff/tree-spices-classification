#  Tree Species Classification using Traditional Machine Learning

This project aims to classify tree species based on image-derived features using traditional Machine Learning techniques. It was built as part of a competitive challenge to showcase effective classification without using deep learning.

## Problem Statement

Given a dataset of tree leaf images, the objective is to correctly classify the species of each tree using handcrafted features and traditional ML algorithms like SVM, Random Forest, etc.

## Dataset

- **Source**: [Kaggle - Tree Species Identification Dataset](https://www.kaggle.com/datasets/viditgandhi/tree-species-identification-dataset)
- **Total Classes**: 15 species
- **Data Format**: Images with labels stored in folders

## 🧪 Approach

### 1. **Preprocessing**
- Resized all images to 64x64 pixels
- Converted to grayscale for simplification
- Flattened into 1D feature vectors

### 2. **Feature Scaling**
- Used `StandardScaler` for normalization

### 3. **Train-Test Split**
- 80-20 split used for model evaluation

### 4. **Models Used**
- Logistic Regression
- Random Forest Classifier
- Support Vector Machine (SVM)

### 5. **Evaluation**
- Accuracy Score
- Classification Report
- Confusion Matrix

##  Results

-  Best Accuracy: **66%**
- Weighted F1-Score: **0.65**
- Notable class-wise performance:
  - `pilikaren`, `other`, and `nilgiri` performed very well
  - `mango` and `asopalav` classes were underrepresented

##  Classification Report Snapshot
precision    recall  f1-score   support

 pilikaren      1.00      1.00      1.00        10
     other      1.00      0.96      0.98        27
    neem        0.55      0.75      0.63        16
 ...
 asopalav       0.00      0.00      0.00         1
   mango        0.00      0.00      0.00         1

Accuracy: 0.66


##  Observations

- **Data Imbalance** negatively affected some classes
- **Traditional ML** worked decently well given simple features
- Accuracy could improve with more feature engineering or deep learning

##  Future Work

- Explore image augmentation to reduce overfitting
- Use texture-based features like LBP or HOG
- Try CNNs for improved performance

## Tech Stack

- Python
- Scikit-learn
- NumPy / Pandas
- Matplotlib / Seaborn
- OpenCV


##  Author

- **Geetha** — [GitHub](https://github.com/she-codesstuff)


