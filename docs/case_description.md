# 📘 Case Description: Ship Mode Sales Normalization

## 🧩 Problem Statement

The original dataset was structured as a cross-tabulated table, with sales values distributed across combinations of `Ship Mode` and `Segment`. This format is not suitable for analysis or visualization in BI tools.

## 🎯 Objective

Transform the cross-tab into a normalized format with one row per transaction, including the following fields:
- `Order ID`
- `Order Date`
- `Ship Mode`
- `Segment`
- `Sales`

## 🛠 Tools & Techniques

- **Power Query (Excel / Power BI)** for data transformation
- **Excel** for initial inspection and validation
- **Documentation** for reproducibility and beginner guidance

## 📈 Outcome

- Clean, normalized dataset ready for BI dashboards and pivot analysis
- Step-by-step guide created to help junior analysts replicate the process
- Screenshots included to illustrate before/after transformation

## 🧠 Learning Value

This case demonstrates:
- How to handle messy, cross-tabulated data
- Practical use of unpivoting and column extraction
- Importance of documentation for auditability and onboarding
