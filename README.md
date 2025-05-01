## README – Inventory Management Analysis (FP20 Challenge 25)

### 🧠 Project Overview
This Power BI report is built for the **FP20 Analytics Challenge 25**, targeting optimization of inventory operations across categories, suppliers, and geographies. The dashboard uses advanced DAX, drill-downs, and smart filtering to surface inefficiencies, supplier risks, and opportunities for restocking strategies.

---

### 📊 Dataset Summary
The dataset contains 5,000 unique products with the following fields:
- Product details (name, category, unit price)
- Stock metrics (quantity, reorder point, stock level)
- Supplier performance (lead time, last restock)
- Geolocation (country, warehouse location)
- Inventory value & restocking behavior

---

## 📈 Dashboard Pages

### 🔹 **Page 1 – Overview**
Focus: High-level KPIs, stock trends, and geographic stock distribution

| KPI | Value |
|-----|-------|
| Total Products | 5,000 |
| Products Below Reorder | 262 |
| Total Inventory Value | ₹1.25 Billion |
| Total Stock Quantity | 3 Million |

**Visual Highlights:**
- Doughnut Chart: Stock Levels (Low: 9.1%, Mid: 40.3%, High: 50.6%)
- Line Chart: Monthly Stock Quantity & Unit Price trends
- Map Visual: Stock distribution across Europe by country & stock level
- Sankey Chart: Product Status breakdown (In Stock: 4,226, Out of Stock: 774)

---

### 🔹 **Page 2 – Deep Dive**
Focus: Supplier performance, pricing, warehouse load, and turnover

| KPI | Value |
|-----|-------|
| Avg Lead Time | 14.96 days |
| Avg Days Since Last Restock (Out of Stock) | 222.38 days |
| Top Supplier by Lead Time | SUP041 (17.3 days) |

**Visual Highlights:**
- Bar Chart: Stock Quantity by Country and Category (Books, Clothing, Electronics)
- Bar Chart: Products per Warehouse (Top: 13 SKUs in AISLE-02-SHELF-03 & AISLE-03-SHELF-11)
- Table: Top 5 Expensive Products (All above ₹998)
- Combo Chart: Turnover Rate vs Min Order Quantity by Category

---

## 🧐 Answers to Analysis Questions

### A. Stock Analysis & Inventory Levels
1. **Top Stocked Category:** Clothing
2. **Products Below Reorder Point:** 262
3. **Minimum Order Quantity Needed:** To be calculated with DAX using `SUMX` across products below reorder

### B. Supplier & Restocking Performance
4. **Top Supplier by Lead Time:** SUP041 (17.3 days)
5. **Avg Days Since Restock (Out of Stock):** 222.38 days
6. **Seasonal Restock Peaks:** March, May, October

### C. Cost & Pricing Analysis
7. **Top 5 Expensive Products:**
   - Product_781 (Books) ₹999.42
   - Product_1565 (Clothing) ₹999.28
   - Product_3842 (Electronics) ₹998.83
   - Product_4810 (Electronics) ₹998.43
   - Product_715 (Electronics) ₹998.30

8. **Fastest Turnover Category:** Sports and Clothing

### D. Warehouse & Geographic Insights
9. **Top Warehouse Location:** AISLE-02-SHELF-03 & AISLE-03-SHELF-11 (13 SKUs each)
10. **Top Countries by Stock:**
   - 1st: Germany
   - 2nd: Spain
   - 3rd: Belgium

---

## 🧰 Business Recommendations
- Restock 262 under-reorder products urgently.
- Monitor suppliers with long lead times (e.g., SUP041) for performance contracts.
- Balance stock across countries and optimize storage space in warehouses.
- Promote or rotate high-value, slow-moving inventory.

---



