# 🚀 **COMPANY SALES ANALYSIS – Excel**

**Advanced Excel project showcasing data analysis, dashboards, and actionable business insights.**

---

## 📊 **Project Overview**

This project demonstrates **advanced Excel skills** through a Sales Dashboard using a realistic dataset:  

- **3,000+ orders**  
- **1,000 customers**  
- **500 products**  

The goal: Analyze sales by **country, product category, and individual products**, while demonstrating **XLOOKUP, IFERROR, Pivot Tables, and charts**.  


💾 Data Cleaning

Some of the data contained empty values, so I removed those rows to focus only on the real, meaningful data. This made sure all calculations, charts, and insights were accurate and reliable.
---

## 🛠️ **Techniques & Formulas Used**

### **1️⃣ XLOOKUP Formulas**

**Pull Customer Country**
```excel
=XLOOKUP(Orders!B2, Customers!A2:A1001, Customers!C2:C1001, "Country not Found", 0)
Matches CustomerID in Orders with Customers sheet

Returns Country or "Country not Found" if missing
```
Pull Customer Name

```excel
=XLOOKUP(B2, Customers!A2:A1001, Customers!B2:B1001, "Customer Not Found", 0)
Retrieves Customer Name and handles missing IDs gracefully
```
Pull Product Category

```excel
=XLOOKUP(C2, Products!A2:A501, Products!C2:C501, "Category Missing", 0)
Matches ProductID to Products sheet

Returns Product Category or "Category Missing" if product not found
```
Total Sales with Error Handling

```excel
=IFERROR(Quantity*UnitPrice,0)
Prevents errors when Quantity or Unit Price is missing
```
**REVENUE BY COUNTRY**
![IMAGE alt](https://github.com/abdulrahman238/COMPANY-SALES-ANALYSIS-EXCEL/blob/4e70dd08c563e3f652ba05a05b320ec131d77ed9/revenue%20by%20country.png)

💡 Key Insights;

🇨🇦 Canada is the top-performing market

🇿🇦 South Africa has the lowest contribution – growth opportunity

Focus marketing and inventory on high-performing countries

**REVENUE BY PRODUCT CATEGORY**
![IMAGE alt](https://github.com/abdulrahman238/COMPANY-SALES-ANALYSIS-EXCEL/blob/54cf83098258224d2146188799f2e87cb0ce9834/product%20category.png)

💡 Key Insights;

Electronics drives the highest revenue

Sports performs strongly in Kenya & South Africa

Helps prioritize inventory, marketing & promotions

Top 10 Performing Products IMAGE
![IMAGE alt](https://github.com/abdulrahman238/COMPANY-SALES-ANALYSIS-EXCEL/blob/8e58abd2cb0c0d5a926247ca8b1feb249f08bb0d/top%2010%20products%20.png)
Takeaways:

Product_459 is the top-selling product

Top 10 products make up ~17.5% of revenue

Guides stocking, bundling, and promotions

**📈 Revenue Distribution Insights by Country & Category**
![IMAGE alt](https://github.com/abdulrahman238/COMPANY-SALES-ANALYSIS-EXCEL/blob/2574faaaa41cc7f3f050e782526c483fa2fe0bbb/precentage%20column.png)

💡 Key Insights;
🌍 Key Observations

Canada shows strong interest in Electronics (30.52%) and Clothing (28.49%), making these two the biggest contributors to Canadian revenue.

Ghana is almost evenly split, with the top categories being Electronics (24.46%), Sports (25.04%), and Home (22.90%) — suggesting a more balanced demand across categories.

In the UK, Clothing (31.58%) and Home (28.63%) dominate, showing a heavy focus on lifestyle-related products.

Kenya has a high contribution from Sports (29.68%) and Electronics (27.42%), which suggests strong demand for active and tech-related items.

Nigeria is driven mostly by Electronics (37.13%), making it the top-performing category in the country by a wide margin.

In the USA, the biggest categories are Home (28.39%), Clothing (25.54%), and Sports (22.13%), showing a mix of household and lifestyle spending.

South Africa also has strong interest in Sports (24.70%) and Food (22.21%), indicating a balance between essentials and recreational items.

🧠 What This Means

Overall, Electronics stands out globally, performing strongly in almost every country. Categories like Sports and Home also perform well in specific regions, while Clothing remains consistently strong across Canada, UK, and USA.



This Project was Created entirely in Excel using XLOOKUP, Pivot Tables, and charts. Summarizes total sales by country, revenue by category, and top-performing products.

