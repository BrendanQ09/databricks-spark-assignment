# 🚀 Databricks Spark Assignment

## 📌 Project Overview
This project is part of **Assignment 3: Spark**, where we analyze IoT device data using **Apache Spark** in **Databricks**. The goal is to **perform data analysis, SQL queries, and machine learning modeling** to gain insights from IoT sensor data.

---

## 📊 Dataset Information
The dataset consists of **IoT device readings**, including:
- **Temperature (`temp`)**
- **Battery Level (`battery_level`)**
- **Humidity (`humidity`)**
- **CO₂ Levels (`c02_level`)**
- **Device Type (`device_name`)**
- **Country (`cn`)**
- **Timestamp (`timestamp`)**

---

## 🔥 Key Analysis & Results

### **1️⃣ SparkSQL Queries**
- **Counted the number of sensor pads from Poland**.
- **Identified distinct LCD colors**.
- **Found the top 5 countries with the most MAC devices**.

### **2️⃣ Machine Learning: K-Means Clustering**
- Used **K-Means Clustering (k=3)** to group devices based on environmental conditions.
- **Key Finding:** Devices with **high CO₂ levels** (Cluster 0) are at **higher failure risk**.
  
| **Cluster** | **Avg Temp (°C)** | **Avg Battery Level** | **Avg Humidity (%)** | **Avg CO₂ Level** | **Insight** |
|------------|------------------|------------------|------------------|------------------|-----------|
| **Cluster 1** (65,931 devices) | **21.99** | **4.50** | **61.9%** | **932.7 ppm** | **Low CO₂, stable conditions** ✅ |
| **Cluster 2** (65,979 devices) | **22.02** | **4.48** | **62.0%** | **1198.97 ppm** | **Moderate CO₂, possible risk** ⚠️ |
| **Cluster 0** (66,254 devices) | **22.02** | **4.51** | **62.1%** | **1466.3 ppm** | **High CO₂, potential failure risk** 🚨 |

---

## 🛠️ Technologies Used
- **Databricks** for data processing
- **Apache Spark (PySpark)**
- **SparkSQL** for querying
- **Machine Learning (MLlib)**
- **Python (Pandas, PySpark ML)**

---

## 📎 How to Use This Notebook
1️⃣ **Clone this repository** or **download the notebook (`.py` or `.dbc` file`)**.  
2️⃣ **Upload the file to Databricks**:
   - Open Databricks and go to **Workspace**.
   - Click **Import** and upload the `.py` or `.dbc` file.  
3️⃣ **Attach the notebook to a running cluster** in Databricks.  
4️⃣ **Run the cells** to explore the dataset and execute the analysis.

---

## 🔗 Project Resources
- **Databricks Published Notebook:** [Click Here](https://databricks.cloud/notebooks/...PasteYourLinkHere)
- **Dataset Source:** [IoT Devices JSON](https://github.com/dmatrix/examples/blob/master/spark/databricks/notebooks/py/data/iot_devices.json)

---

## 📌 Author
👤 **BrendanQ09**  
📅 **Date:** March 2025  
📬 **Email:** [Your Email Here]  

---

### ⭐ If you found this project helpful, consider giving it a star! ⭐
