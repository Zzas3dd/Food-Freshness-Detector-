 # 🍎 Fresh vs Rotten Fruits Classification & Clustering

This project implements machine learning techniques to classify fruit images as **fresh or rotten**, and to explore patterns in the data using **clustering algorithms**.

The work is done entirely in a Jupyter Notebook and includes **data preprocessing, classification, and clustering**.

---

## 📌 Overview

The project uses a dataset of fruit images and converts them into **numeric pixel arrays** to train machine learning models.

It includes:
- Data preprocessing and cleaning
- Binary classification (fresh vs rotten)
- Multiclass classification (fruit + condition)
- Unsupervised clustering (K-Means and DBSCAN)
- Model evaluation using standard metrics

---

## 🍌 Supported Fruits

The dataset (and model) includes only:

- Apple 🍎  
- Banana 🍌  
- Orange 🍊  

Each image belongs to one of:
- **Fresh**
- **Rotten**

---

## 🧠 Tasks Implemented

### 1. Data Preparation
- Load dataset from Kaggle  
- Organize images into a DataFrame  
- Convert images into numeric pixel arrays  
- Encode labels  
- Split into training and testing sets  
- Scale features using `StandardScaler`  

---

### 2. Binary Classification
- **Goal:** Classify fruit as fresh or rotten  
- **Model:** Neural Network (Keras Sequential)  
- **Optimizer:** Adam  

---

### 3. Multiclass Classification
- **Goal:** Classify into specific categories such as:
  - Fresh Apple  
  - Rotten Banana  
  - Fresh Orange  

- **Model:** Neural Network (Keras Sequential)  
- Labels encoded using `LabelEncoder` and `to_categorical`  

---

### 4. Clustering (Unsupervised Learning)

#### K-Means
- Groups images based on similarity  
- Evaluated using silhouette score  

#### DBSCAN
- Density-based clustering  
- Identifies clusters and noise points  

---

## 📊 Evaluation Metrics

The models are evaluated using:

- Accuracy  
- Precision  
- Recall  
- F1-score  
- ROC-AUC  
- Confusion Matrix  
- Classification Report  

Clustering is evaluated using:
- Silhouette Score  

---

## 🏗️ Technologies Used

- Python  
- NumPy  
- Pandas  
- Matplotlib / Seaborn  
- PIL (Image processing)  
- Scikit-learn  
- TensorFlow / Keras  

---

## ⚙️ Dataset

The dataset is downloaded using Kaggle:

sriramr/fruits-fresh-and-rotten-for-classification

It contains labeled images organized into folders such as:

- freshapples  
- rottenapples  
- freshbanana  
- rottenbanana  
- freshoranges  
- rottenoranges  

---

## 🔍 How It Works

1. Images are loaded from dataset folders  
2. Each image is converted into a numeric array  
3. Data is scaled and preprocessed  
4. Models are trained:
   - Binary classifier (fresh vs rotten)  
   - Multiclass classifier (fruit + condition)  
5. Clustering algorithms group similar images  
6. Results are evaluated using metrics and visualizations  

---

## 🚫 Limitations

- Only supports **apple, banana, and orange**  
- Works on **image datasets only** (no real-time input)  
- Model performance depends on dataset quality  
- No deployment (not an API or app)  

---

## 🔮 Future Improvements

- Add more fruit categories  
- Use CNNs instead of basic dense networks  
- Improve accuracy with better preprocessing  
- Add visualization of clusters  
- Deploy as a web or mobile application  
