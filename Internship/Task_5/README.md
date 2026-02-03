
# California House Price Prediction

## 📖 Project Overview
This project focuses on predicting house prices in California using a real-world housing dataset.  
The dataset contains **20,000 data entries** with various numerical and categorical features related to housing conditions.

The main objectives of this project are:
- To handle missing values effectively using **Simple Imputer (Median strategy)**
- To perform **Exploratory Data Analysis (EDA)** to understand data patterns
- To prepare clean data for building a **house price prediction model**

---

## 📂 Dataset Information
- Dataset: California Housing Dataset
- Number of records: ~20,000
- Target variable: House Price
- Features include:
  - Median income
  - Housing age
  - Number of rooms
  - Population
  - Location-based attributes

---

## 🧹 Data Preprocessing
### Handling Missing Values
- Missing values were handled using **Simple Imputer**
- Strategy used: **Median**
- Median was chosen because:
  - It is robust to outliers
  - It preserves the central tendency of skewed data

```python
from sklearn.impute import SimpleImputer

imputer = SimpleImputer(strategy="median")
data_imputed = imputer.fit_transform(data)
