# 🚇 Delhi Metro Data Analysis Project

## 📌 Project Overview
This project performs end-to-end **data cleaning**, **feature engineering**, and **visual analysis** on Delhi Metro transaction data. The goal is to extract meaningful insights related to station performance, passenger movement, revenue, and profitability.

---

## 📂 Dataset
The dataset used in this project:

👉 **[Download delhi_metro_cleaned_data.csv](./delhi_metro_cleaned_data.csv)**


It contains columns such as:

- Ticket_Type  
- From_Station  
- To_Station  
- Passenger_Count  
- Cost  
- Revenue  
- Other numerical and categorical attributes

(Columns are based on the fields processed in the notebook.)

---

## 🧹 Data Cleaning & Preprocessing

### ✅ 1. Handling Missing Values
- Identified **three columns** with null values.
- Performed:
  - **Mode imputation** for `Ticket_Type`
  - **Median imputation** for numerical columns
- After this, only **one column** remained with NaN values, which was also filled with its median.

### ✂️ 2. Removing Trailing Spaces
- The `From_Station` column contained trailing spaces.
- Cleaned using `.str.strip()`.

### 🔢 3. Feature Engineering
Created an additional feature:


---

## 📊 Data Visualization
The following visual analyses were performed using **Matplotlib** and **Seaborn**:

### 📈 Distribution Analysis
- Histogram of passenger counts  
- Distribution of ticket types  
- Profit distribution  

### 🔍 Relation Analysis
- Revenue vs Passenger Count  
- Profit vs Station  
- Ticket Type vs Revenue  

### 📍 Station-Level Insights
- Most popular originating stations  
- Most popular destination stations  
- Highest profitable routes  

---

## 🛠️ Technologies Used
- **Python 3**
- **Pandas**
- **NumPy**
- **Matplotlib**
- **Seaborn**
- **Jupyter Notebook**

---

## 🚀 How to Run This Project

### 1. Clone the repository
```bash
git clone <your-repository-url>
cd delhi-metro-analysis
```
### 2. Install dependencies
```bash
pip install -r requirements.txt
```

### 3. Launch Jupyter Notebook
```bash
jupyter notebook

Open the file:
Delhi-Metro-Analysis.ipynb



