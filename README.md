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

📈 Charts & Dashboard
Bar Chart: Total Sales by Country

Column/Pie Chart: Revenue by Product Category

Column Chart (Top 10 Products): Highlights top products by revenue

Dashboard Image
![Dashboard Image](./images/dashboard.png)


Created entirely in Excel using XLOOKUP, Pivot Tables, and charts. Summarizes total sales by country, revenue by category, and top-performing products.

