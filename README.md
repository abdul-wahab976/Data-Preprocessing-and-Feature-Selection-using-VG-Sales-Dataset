# 🎮 Lab 4: Data Preprocessing and Feature Selection using VG Sales Dataset

This project focuses on **data preprocessing** and **feature selection** using the **VG Sales Dataset**.  
The main objective is to clean, transform, and prepare the dataset for **data mining** and **machine learning tasks**.

---

## 📋 Steps Performed

### 1️⃣ Data Description
- Loaded the **VG Sales dataset** using pandas.  
- Displayed **dataset shape**, **column names**, and **data types**.  
- Identified **numerical** and **categorical** features.  
- Checked for **missing values**, **duplicates**, and **unique counts** per column.  

---

### 2️⃣ Data Cleaning
- Replaced invalid or missing values (**NaN or blanks**) with appropriate strategies:
  - Mode for **categorical columns**  
  - Mean/Median for **numerical columns**  
- Removed **duplicate rows**.  
- Standardized column names (e.g., lowercase, underscore format).  

---

### 3️⃣ Handling Noisy Data
- Detected **outliers** using the **IQR method**.  
- Replaced outliers with the **median value** of the column.  
- Fixed inconsistent categorical entries (e.g., typos or mixed casing).  

---

### 4️⃣ Feature Encoding
- Applied **Label Encoding** for categorical columns.  
- Converted **textual categories** into **numerical form** for ML compatibility.  

---

### 5️⃣ Feature Selection
Used **statistical methods** to check feature relevance:
- **Variance Threshold** → removed low-variance features  
- **Correlation Analysis**:
  - Pearson correlation → for numerical features  
  - Chi-Square test → for categorical features  

**Visualized relationships using:**
- Correlation Heatmap  
- Pairplot  
- Chi-Square Crosstab Heatmap  

---

### 6️⃣ Data Normalization
Scaled **numerical columns** using:
- **MinMaxScaler** (range 0–1) or  
- **StandardScaler** (z-score normalization)

---

## 📊 Visualizations
- 🔥 **Correlation Heatmap** – shows relationships between numerical variables  
- 📦 **Boxplots** – identify and visualize outliers  
- 📈 **Crosstab Heatmap** – explore categorical relationships  
- 🌀 **Pairplot** – view numerical variable interactions  

---

## ⚙️ Libraries Used
```python
pandas  
numpy  
matplotlib  
seaborn  
scikit-learn  
scipy
