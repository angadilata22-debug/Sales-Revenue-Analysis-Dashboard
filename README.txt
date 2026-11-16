SALES & REVENUE ANALYSIS DASHBOARD
=================================

PROJECT OVERVIEW
This project analyzes a sample retail sales dataset and presents sales performance through KPIs, monthly trends, product performance, and interactive filters.

FILES
-----
1. Sales_Dataset.csv       - Source data for Power BI or Excel.
2. Sales_Dashboard.xlsx    - Excel workbook with Sales Data and Dashboard sheets.
3. PowerBI_Theme.json      - Optional Power BI report theme.
4. PowerBI_Guide.pdf       - Step-by-step instructions for building the report in Power BI.

DATASET FIELDS
--------------
OrderID, OrderDate, Product, Category, Region, Quantity, UnitPrice, Revenue, Cost, Profit, Salesperson.

Revenue = Quantity x UnitPrice
Profit  = Revenue - Cost

EXCEL DASHBOARD
---------------
Open Sales_Dashboard.xlsx in Microsoft Excel. Go to the Dashboard sheet.
Use the Region Filter and Category Filter dropdowns in cells B3 and E3.
The KPI cards and summary tables use formulas and update when filters are changed.
If formulas do not show immediately, open the file in Excel and press Ctrl+Alt+F9 to recalculate.

POWER BI BUILD STEPS
--------------------
1. Open Power BI Desktop.
2. Select Home > Get data > Text/CSV.
3. Choose Sales_Dataset.csv and select Load.
4. In Data view, confirm OrderDate is Date and Revenue/Cost/Profit are Decimal Number.
5. Create measures using the DAX expressions in PowerBI_Guide.pdf.
6. Add four Card visuals: Total Revenue, Total Orders, Units Sold, Total Profit.
7. Add a Line chart: Axis = OrderDate (Month); Values = Total Revenue.
8. Add a Clustered bar chart: Axis = Product; Values = Total Revenue.
9. Add a Donut chart: Legend = Category; Values = Total Revenue.
10. Add slicers for Region, Category, and OrderDate.
11. Apply PowerBI_Theme.json using View > Themes > Browse for themes.
12. Save your report as Sales_Revenue_Analysis.pbix.

NOTE
----
The dataset is synthetic sample data created for this assignment. Replace it with real business data if your instructor has provided a dataset.
The Excel workbook is provided as a ready-to-use interactive template. Native Power BI slicers are created inside Power BI Desktop using the steps in the guide.
