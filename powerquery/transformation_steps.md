# 🔧 Power Query Transformation Steps

This guide outlines the exact steps used to normalize the cross-tabulated sales table. Each step is documented to ensure reproducibility and clarity for beginners.

## 🧭 Overview

- Source file: `raw_dirty_sales_table.xlsx`
- Goal: Convert a cross-tab format into a normalized table with columns: `Order ID`, `Order Date`, `Ship Mode`, `Segment`, `Sales`

---

## 🪜 Steps

### 1. Load Data
- Open Excel and launch Power Query.
- Load the raw table from `raw_dirty_sales_table.xlsx`.

### 2. Remove Empty Rows and Columns
- Filter out blank rows and columns to isolate the actual data.

### 3. Promote Headers
- Use the first row as column headers.

### 4. Unpivot Segment Columns
- Select all columns representing `Segment` values under each `Ship Mode`.
- Apply **Unpivot Columns** to convert them into attribute-value pairs.

### 5. Extract `Ship Mode` and `Segment`
- Split the column names (e.g., `Standard Class - Home Office`) into two separate fields:
  - `Ship Mode`
  - `Segment`

### 6. Rename Columns
- Ensure consistent naming:
  - `Attribute` → `Ship Mode`
  - `Segment` → `Segment`
  - `Value` → `Sales`

### 7. Change Data Types
- Convert `Sales` to decimal or currency.
- Ensure `Order Date` is in date format.

### 8. Final Cleanup
- Remove duplicates (if any).
- Sort by `Order Date` or `Order ID` as needed.

---

## ✅ Output

A normalized table ready for analysis and visualization in BI tools.
