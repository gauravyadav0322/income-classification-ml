# income-classification-ml

# Income Prediction using Machine Learning

This project predicts whether an individual's income exceeds a certain threshold (>50K) based on demographic and socio-economic attributes. The dataset closely resembles the UCI Adult Census dataset.  
The workflow includes data cleaning, exploratory analysis, feature engineering, model building, and evaluation.

---

## 📁 Project Structure
- **Predicting_Income.ipynb** – Full workflow notebook with EDA, preprocessing, model training & evaluation  
- **income dataset.csv** – Raw dataset used for training the model  

---

## 📊 Key Steps in the Project

### **1. Exploratory Data Analysis (EDA)**
- Inspected missing values & data types  
- Visualized categorical distributions  
- Analyzed age, education, occupation, work hours, capital gain/loss, etc.  
- Identified insights such as:
  - Dropout patterns (educational-num ≤ 5)
  - High capital gain/loss groups
  - Work hours vs occupation patterns  

### **2. Feature Engineering**
- Converted educational-num ≤ 5 into a new category: `dropout`
- Created new flags:
  - `good investor` (capital-gain > 1)
  - `bad investor` (capital-loss > 1)
- Encoded categorical variables
- Normalized numerical features where required  

---

## 🤖 Machine Learning Models Used
- Logistic Regression  
- Decision Trees  
- MLP Classifier (Neural Network)  
- Additional evaluation techniques such as:
  - Classification Report  
  - Confusion Matrix  

---

## 📈 Model Evaluation
Models were evaluated using:
- Accuracy  
- Precision  
- Recall  
- F1-score  

---

## 🔧 Technologies Used
- Python  
- NumPy  
- Pandas  
- Matplotlib / Seaborn  
- Scikit-learn  
