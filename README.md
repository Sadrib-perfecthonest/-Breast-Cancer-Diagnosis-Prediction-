# 🩺 Breast Cancer Diagnosis Prediction  
**Machine Learning Project using K-Means Clustering & K-Nearest Neighbors (KNN)**  

This project predicts whether a breast tumor is **Malignant (M)** or **Benign (B)** using both **unsupervised** and **supervised** learning methods. By applying **K-Means Clustering** and **K-Nearest Neighbors (KNN)** on the Wisconsin Diagnostic Breast Cancer (WDBC) dataset, we evaluate how well these algorithms perform in medical diagnosis tasks.

---

## 📋 Project Overview  
Breast cancer detection is a critical real-world application of machine learning.  
This project aims to:

- ✔️ Apply **K-Means (Unsupervised)** and **KNN (Supervised)**  
- ✔️ Compare clustering vs. classification approaches  
- ✔️ Achieve high accuracy in diagnosis prediction  
- ✔️ Build reproducible and deployable ML models using **Flask + HTML/CSS**  

The project notebook includes complete steps: Data cleaning → EDA → Model building → Evaluation → Model saving.

---

## 🎯 Objectives  
- Use **K-Means Clustering** to understand natural grouping of tumors  
- Build **KNN Classifier** for supervised cancer diagnosis  
- Compare the performance and accuracy of both approaches  
- Serialize trained models using **joblib**  
- Deploy prediction model using **Flask** and a simple web interface  

---

## 📊 Dataset Information  
**Source:** Wisconsin Diagnostic Breast Cancer (WDBC)  
**Samples:** 569 tumor cases  
**Features:** 30 numerical features (radius, texture, perimeter, area, smoothness, etc.)  
**Target:**  
- **M** = Malignant  
- **B** = Benign  

### 🔢 Class Distribution  
| Class | Count | Percentage |
|-------|--------|------------|
| Benign (B) | 357 | 62.7% |
| Malignant (M) | 212 | 37.3% |

Balanced enough for machine learning, but still with slight class imbalance.

---

## 🔧 Technologies Used  
### **Programming Language**
- Python 3.8+

### **Libraries**
- **pandas**, **numpy** – Data handling  
- **matplotlib**, **seaborn** – Visualization  
- **scikit-learn** – ML algorithms (KNN, K-Means, scaling, splitting)  
- **joblib** – Model saving  
- **Flask**, **HTML**, **CSS** – Deployment  

---

# 🤖 Machine Learning Algorithms Explained  

## 🔍 K-Nearest Neighbors (KNN) – *Supervised Classification*  
KNN is one of the simplest yet powerful classification algorithms.  
It works by:

1. Calculating the distance between the test sample and all training samples  
2. Selecting the **K nearest** neighbors  
3. Using **majority vote** to predict the class  

### **Why KNN works well here**
- Breast cancer dataset is numerical and well-separated  
- KNN captures local patterns effectively  
- High accuracy with minimal tuning  

### **Pros**
- Simple and intuitive  
- No training time (lazy learner)  
- Highly accurate for small/medium datasets  

### **Cons**
- Slow for large datasets  
- Sensitive to irrelevant features → scaling required  

---

## 🎛️ K-Means Clustering – *Unsupervised Learning*  
K-Means is a clustering algorithm that groups data into **K clusters**.

It works in 3 steps:

1. Randomly choose K centroids  
2. Assign each data point to its nearest centroid  
3. Recalculate centroids and repeat  

### **Why K-Means is used here**
Even without labels, K-Means can discover natural structure in the data and separate benign vs malignant tumors reasonably well.

### **Pros**
- Fast and efficient  
- Finds hidden structure in data  
- No labels required  

### **Cons**
- Requires selecting K manually  
- Struggles if clusters overlap  

---

# ⭐ Key Findings  
### 📌 KNN Performance  
- **High supervised accuracy**  
- Consistent predictions on unseen test data  
- Best choice for this medical classification task  

### 📌 K-Means Performance  
- Achieved ~**86% accuracy** without labels  
- Shows strong natural separation of tumor types  
- Good for dataset understanding  

---

## 🛠️ Future Enhancements  
- 🔄 Add **cross-validation** for more robust evaluation  
- 🌲 Implement **ensemble methods** such as Random Forest and XGBoost  
- 📊 Add **feature importance analysis** to understand key predictors  
- 🌐 Create an interactive **web interface** for easy predictions  
- 🖼️ Integrate with **medical imaging systems** for end-to-end diagnostic workflows  

---


## 📄 License  
This project is created for **educational purposes**.  
The dataset is publicly available from the **UCI Machine Learning Repository**.

---

## 🧪 Running the Notebook  
   - Clone the repository
   - Navigate to the project directory
   - Launch Jupyter Notebook
     
