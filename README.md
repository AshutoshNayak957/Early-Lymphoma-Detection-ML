## 📌 Project Overview
This project applies machine learning techniques to classify lymphoma cancer types using **high-dimensional gene expression data**.  
The dataset contains **4000+ gene expression features** for a small number of patient samples.

The goal is to **predict the type of lymphoma** accurately, helping in **early detection** and supporting medical diagnosis.

---

## 🎯 Problem Statement
- **Input:** Gene expression values (~4000 features)  
- **Output:** Cancer type (DLBCL, FL, etc.)  
- **Challenge:** Small sample size & high-dimensional data, prone to overfitting  

> "The dataset suffers from the curse of dimensionality, making feature selection and dimensionality reduction critical."

---

## ⚙️ Techniques & Workflow
1. **Data Preprocessing**
   - Handling missing values with `SimpleImputer`
   - Encoding categorical target labels
   - Standardizing features with `StandardScaler`
2. **Dimensionality Reduction**
   - Principal Component Analysis (PCA)  
   - Reduced features from 4026 → 50–95% variance retained
3. **Machine Learning Models**
   - Random Forest
   - Support Vector Machine (**best model**)
   - K-Nearest Neighbors (KNN)
   - Logistic Regression
4. **Evaluation Metrics**
   - Accuracy
   - Precision
   - Recall
   - F1-score
   - Confusion Matrix
   - Cross-validation (5-fold)
5. **Visualization**
   - PCA 2D scatter plot
   - Confusion matrix heatmap
   - Model comparison bar chart
   - Feature importance plot

---

## 📊 Results

| Model | Accuracy |
|-------|---------|
| SVM (Linear) | 100% |
| KNN | 100% |
| Logistic Regression | 100% |
| Random Forest | 78.6% |

**Cross-validation Accuracy (SVM):** 100%  

> The SVM model achieved perfect classification, indicating strong separation in gene expression features.

---

## 📈 Visualizations

1. **PCA 2D Plot**

![PCA Plot](images/pca_plot.png)

2. **Confusion Matrix**

![Confusion Matrix](images/confusion_matrix.png)

3. **Model Comparison**

![Model Comparison](images/model_comparison.png)

4. **Top 10 Important Genes (Random Forest)**

![Feature Importance](images/feature_importance.png)

> *Tip: Save your graphs in an `images/` folder to display here.*

---

## 🧠 Key Insights
- PCA helped reduce dimensionality, improving model generalization.
- SVM performed best due to high-dimensional feature handling.
- High accuracy indicates gene expression patterns are strong predictors of lymphoma types.

---

## 🚀 Future Scope
- Use larger datasets for better generalization  
- Apply deep learning methods (e.g., CNN or Autoencoders)  
- Develop a web application to allow doctors to upload gene data for instant prediction  

---

## 📁 Folder Structure

```text
Lymphoma-ML-Project/
│── project.ipynb          # Notebook with full code
│── Lymphoma.arff          # Dataset
│── README.md              # Project description
│── images/                # Graphs for README
│    ├── pca_plot.png
│    ├── confusion_matrix.png
│    ├── model_comparison.png
│    └── feature_importance.png
