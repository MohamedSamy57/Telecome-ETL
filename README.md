# ETL Project for Telecom Company

---

## 📌 Project Description
This ETL project was designed to handle and process telecom data using **SQL Server Integration Services (SSIS)**. 

🔹 Extracts data from CSV files
🔹 Transforms it according to specific rules
🔹 Loads it into a structured database

The objective is to ensure **data quality** and facilitate **analysis**.

---

## 🎯 Project Values
✅ **Data Accuracy**: Ensuring valid and clean data is stored in the database.  
✅ **Automation**: Automating data processing at regular intervals.  
✅ **Error Handling**: Managing rejected records separately for quality control.  
✅ **Scalability**: Designed to handle increasing volumes of telecom data efficiently.  

---

## 📂 Data Source
The data is provided in **CSV format**, containing records of telecom transactions every **5 minutes**.

📌 The dataset includes:
- **IMSI**
- **IMEI**
- **CELL**
- **LAC**
- **EVENT_TYPE**
- **Timestamps**
  
![5](https://github.com/user-attachments/assets/b55c9e72-0559-4695-adbc-4603040f8c63)

---

## 🛠 Tools
🔹 **SQL Server Integration Services (SSIS)** - ETL process implementation  
🔹 **SQL Server** - Data storage and querying  
🔹 **CSV Files** - Source of raw transaction data  

---

## 📦 Package Design
The **SSIS package** follows a structured approach:

### 1️⃣ Extract
📌 Reading data from CSV files

### 2️⃣ Transform
- Cleaning and standardizing data
- Validating timestamps and rejecting malformed records
- Splitting **IMEI** values into **TAC and SNR**
- Enriching data by mapping **IMSI** to a subscriber ID

### 3️⃣ Load
📌 Inserting valid data into a **SQL Server database**

### 4️ Moving
📌 Moving Files to another **Directory**

<p align="center">
  <img src="https://github.com/user-attachments/assets/0edfa4af-d515-432f-b973-90ef897bd036" alt="ETL Project Image" width="500">
</p>

---
![2_page-0001 (1)](https://github.com/user-attachments/assets/89e83351-f091-4f1d-a543-51a11dde7b1d)

---

## 🔄 Control Flow
🔹 **Scheduled execution** every 5 minutes to process new data files  
🔹 **Error handling mechanism** to store rejected records separately  
🔹 **Logging and monitoring** steps for tracking ETL execution  

---

## 🔀 Data Flow
📌 **Extracted from CSV** ➡ **Transformed with rules** ➡ **Loaded into the database**

🛠 **Data transformation includes:**
- ✅ Null checks and rejections for invalid records
- ✅ Substring operations on IMEI values
- ✅ Mapping IMSI to subscriber IDs
- ✅ Timestamp validation

---

## 🏛 Database Schema Design
📂 **Transaction Table** - Stores validated records  
📂 **Rejected Records Tables** - Stores invalid records for review  
📂 **Reference Tables** - Contain lookup values for mapping operations  

![7](https://github.com/user-attachments/assets/318f8743-764c-47e2-84f5-681e21b49d02)

---
## 📊 Result
The ETL pipeline ensures **structured and reliable data storage**, improving the **efficiency of telecom data processing**.  

✅ Clean, validated, and ready-for-analysis dataset  
✅ Insights into **network activities** and **customer interactions**  

![6](https://github.com/user-attachments/assets/6e57c79b-2ef0-475d-8bf0-4ecc9b7a3d50)

---

## 📌 Conclusion
This ETL project ensures efficient telecom data processing, reducing errors and improving **data accuracy**.  
By automating the data pipeline, it **saves time**, enhances **scalability**, and provides **actionable insights** for decision-making.  
With this setup, telecom companies can **streamline operations** and **improve service quality**. 🚀  

---
