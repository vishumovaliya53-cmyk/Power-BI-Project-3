# 📊 Power BI Sales Analysis Project

## 📌 Introduction
This project focuses on analyzing sales data using Microsoft Power BI.  
The main objective is to understand business performance and apply DAX functions to generate meaningful insights.

---

## 🗂️ Data Model
The project follows a **star schema** with one fact table and multiple dimension tables:

- Sales_Fact  
- Customer_Dim  
- Product_Dim  
- Region_Dim  
- Date_Dim  
- Returns_Fact  

---

## 🧮 Calculated Columns
- **Profit** = SalesAmount - Cost  
- **ReturnFlag** → Identifies returned and non-returned transactions  
- **Customer Full Name** → Combination of First Name and Last Name  

---

## 📈 Measures Created
- Total Sales  
- Total Cost  
- Total Profit  
- Return Rate (%)  
- Average Sale per Transaction  

---

## ⚡ Quick Measures
- Year-over-Year (YoY) Sales Growth  
- Difference between Current Month and Previous Month Sales  

---

## 🧾 Measure Management
- Created a dedicated **Measures Table**  
- Helps in organizing all DAX measures in one place  

---

## 🔍 Filter Context Analysis
Used the following DAX functions to understand filter behavior:

- `ALL()` → Removes filters  
- `FILTER()` → Applies custom filters  
- `CALCULATE()` → Modifies filter context  

---

## 🧠 DAX Functions Used

### 📊 Mathematical Functions
- SUM, AVERAGE, MAX  

### 🔢 Counting Functions
- COUNTX, DISTINCTCOUNT  

### 🧩 Logical Functions
- IF, AND, OR, SWITCH  

### 🔤 Text Functions
- CONCATENATE, UPPER, LEFT  

### 📅 Date Functions
- YEAR, MONTH, EOMONTH  

---

## 🔗 Relationships
- Established relationships between fact and dimension tables  
- Used `RELATED()` function to fetch:
  - Customer Name  
  - Product Name  
  - Region Details  

---

## ⏳ Time Intelligence
- TOTALYTD()  
- SAMEPERIODLASTYEAR()  
- DATESINPERIOD()  
- Running Total using CALCULATE() and DATESBETWEEN()  

---

## 🚀 Additional Scenarios
- Categorized sales into **Low, Medium, High** using `SWITCH()`  
- Used `SUMX()` and `AVERAGEX()` for advanced row-based calculations  

---

## 🏁 Conclusion
This project demonstrates the practical use of Power BI for data analysis.  
It highlights how data modeling, DAX calculations, and visualizations help in generating business insights and improving decision-making.

---