# 📊 Tableau Dashboard – Visual Analytics Problem Set #6 

This Tableau project includes three dashboards developed as part of  Visual Analytics, showcasing techniques like **persistent Set Actions**, **shape icon filtering**, **Level of Detail (LOD) expressions**, and **custom tooltip logic**. Each dashboard is tailored for rich user interactivity and precision storytelling with data.

---

## 📁 Files Included

| File | Description |
|------|-------------|
| `Problem_Set_6_Dashboard.twbx` | Tableau workbook with all three dashboards |
| `dashboard_screenshots/` | Optional folder for preview images of each dashboard |

---

## 🟩 Problem 1 – Persistent State Selector + Icon Filters (Coffee Chain)

**Dataset:** Coffee_Chain_Updated

🧠 **Objective:**  
Enable users to interactively select states and product types using persistent Set Actions and shape-based icon filters.

🔧 **Techniques Used:**
- Set Action: **Keep values on clearing selection**
- State List with dynamic "x" labels using `"x " + [State]`
- Created four sets for **Product Type**: Coffee, Espresso, Herbal Tea, Tea
- Built **shape charts** with ✓ (IN) and ○ (OUT) using custom shapes
- Added shape sheets to a vertical container as clickable filters
- Used combined `Selected Types` calculated field to filter the main charts

🎯 **Result:**  
A clean, interactive dashboard that lets users select states and filter product types with icon-based toggles — all driven by persistent set actions and custom filtering logic.

---

## 🗺️ Problem 2 – Donor Map with LOD & Null Handling

**Datasets:**  
- Advancement_donations_and_giving_Combined.xlsx  
- Mapping_US.xlsx

🧠 **Objective:**  
Create a stylized USA map using square marks to visualize the **number of donors** and **total donation amount** from each state.

🔧 **Techniques Used:**
- Shape chart using filled squares from `Mapping_US` grid
- LOD Calculation for **Distinct Donors per State**
- `ZN()` function to convert null donation values to 0
- Custom **color scale** ranging from $0 to $3.2M
- Tooltip formatting:
  - If no donors: show "0 donors\nTotal Donated: $0"
  - Otherwise, display actual values in currency format

🎯 **Result:**  
A visually engaging donor heatmap that includes all states, gracefully handles missing data, and supports strategic advancement insights.

---

## 📅 Problem 3 – Customer Lifecycle Retention Table

**Dataset:** Sample - Superstore

🧠 **Objective:**  
Track customer acquisition and retention across years using LOD to identify first purchase year and build comparative tables.

🔧 **Techniques Used:**
- LOD Field: `Yr-StartedPurchasing` = `{FIXED [Customer Name] : MIN(YEAR([Order Date]))}`
- First Table: Count of customers by `Yr-StartedPurchasing` and `Order Date (Year)`
- Second Table: % breakdown of New vs. Continuing customers per year
- Used Totals and Table Layout formatting
- Tooltips with calculated fields explaining customer behavior

🎯 **Result:**  
A dual-table dashboard that reveals how many customers are retained over time, supporting customer lifecycle and loyalty analysis.

---

## 💡 Key Tableau Concepts Demonstrated

- ✅ Persistent Set Actions for selection memory
- ✅ Shape mark filters (✓ / ○) using Sets
- ✅ Level of Detail (LOD) calculations (`FIXED`)
- ✅ Handling nulls with `ZN()` for donation values
- ✅ Custom tooltips, formatted legends, and conditional logic
- ✅ Layout containers and visual alignment techniques

---

## 📫 Connect with Me

- 🌐 [LinkedIn – Praneth Nandeesh](https://www.linkedin.com/in/praneth-nandeesh-789038285/)
- 📊 [Kaggle Dashboards](https://www.kaggle.com/pranethhh)
- 📧 Email: pranethnandeesh@gmail.com

---

## 📌 License

This project was developed as part of MAX 507 coursework at Illinois Tech and is shared for educational and portfolio use.

