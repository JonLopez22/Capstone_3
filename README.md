# Capstone 3: Analysis with Power BI
**Year Up United Data Analytics Training Academy - Week 12**
**Analyst:** Jonathan Lopez | **Region:** NorthEast (Maryland, Massachusetts, Maine & New Jersey)

---

## Project Overview

This project analyzes four years of sales data (2022-2025) for the **Northeast Region** of EmporiUm, a virtual student bookstore operating both in-store and online locations. The report was built in Power BI Desktop and is designed to be shared with the Northeast Region's director, territory managers, and individual store managers to support data-driven business decisions.

The analysis covers in-store locations across **Maryland**, **Massachusetts**, **Maine**, and **New Jersey**, as well as online orders shipped to those states.

---

## Data Sources

| File | Description |
|------|-------------|
| 'Capstone3_Sample_Sales.xlsx' | Main data workbook containing in-store sales, online sales, product catalog, store locations, and management hierarchy |
| 'book_list.txt' | Reference list of 90 general-audience book titles and their authors used to enrich the top-selling books visual |

### Sheets Used from Excel Workbook
- **Store Sales** - In-Store transaction records (Transaction Date, Store ID, Product, Category, Sale Amount)
- **Online Sales** - Online order records (Year, Month, Day, Product, Sales Total, Ship-to-State)
- **Products** - Product catalog with category and subcategory classifications
- **Store Locations** - Maps Store IDs to city and state for filtering and geographic analysis

---

## Report Pages

### Page 1 - Sales Overview
- **Line Chart:** Sales trend over the full 2022-2025 period, comparing in-store vs online sales
- **Donut Chart:** Sales distribution by State
- **Slicer:** Interactive filter by year

---

### Page 2 - Sales by Category
- **Column Chart:** Sales performance by Product category, sorted by revenue
- **Table:** Top-selling general-audience books with author names (textbooks excluded)

---

## Data Cleaning & Modeling Highlights
- Merged Year/Month/Day columns in Online Sales into a single Date column using Power Query
- Resolved null Category values in Store Sales (Art Supplies products imported as #N/A)
- Normalized column names across both fact tables and appended into a unified Sales table
- Filtered data to Northeast Region only (Store IDs 730-739, 801-823, 824-839 for in-store;
MD, MA, ME, NJ for online)
- Built a custom DAX Calender table spanning 2022-2025 with Year, Month, Quarter columns
- Joined book list reference file to Products table to add author names to the books visual

---

## Video Walkthrough

*Link will be added upon completion of video recording.*

---

## Repository Contents

```
Capstone_3/
|
|--- Lopez_Capstone3.pbix           # Power BI report file
|--- Capstone3_Sample_Sales.xlsx    # Source data workbook
|--- book_list.txt                  # Book titles and authors reference file
|--- README.md                      # This file
```
---

## Tools Used
- Power BI Desktop (Power Query, DAX, Model View)
- GitHub / Git Bash
- Microsoft Excel
