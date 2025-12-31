# 🚀 **COMPANY  SALES ANALYSIS – Excel**

**Advanced Excel project showcasing data analysis, dashboards, and actionable business insights.**

---

## 📊 **Project Overview**

This project demonstrates **advanced Excel skills** through a Sales Dashboard using a realistic dataset:  

- **3,000+ orders**  
- **1,000 customers**  
- **500 products**  

The goal: Analyze sales by **country, product category, and individual products**, while demonstrating **XLOOKUP, IFERROR, Pivot Tables, and charts**.  

---

## 🛠️ **Techniques & Formulas Used**

### **1️⃣ XLOOKUP Formulas**

**Pull Customer Country**
```excel
=XLOOKUP(Orders!B2, Customers!A2:A1001, Customers!C2:C1001, "Country not Found", 0)

**Pull Product Category**
=XLOOKUP(C2, Products!A2:A501, Products!C2:C501, "Category Missing", 0)
