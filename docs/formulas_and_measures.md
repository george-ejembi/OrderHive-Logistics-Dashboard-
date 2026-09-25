# Key Formulas and Measures

This document outlines the core Excel formulas and Power Pivot/DAX measures used to calculate the KPIs in the OrderHive Logistics Dashboard.

##  Core KPI Calculations

### Total Orders
- **Formula:** `=COUNTA(Data[Order_ID])` or `=SUM(Data[Order_Count])`
- **Purpose:** Calculates the total volume of orders placed (72.32K).
- **Logic:** Counts all unique order IDs in the dataset.

### Gross Order Revenue
- **Formula:** `=SUM(Data[Gross_Revenue])`
- **Purpose:** Calculates total revenue before deductions ($6,786,304).

### On-Time Orders
- **Formula:** `=COUNTIFS(Data[SLA_Breach], 0)`
- **Purpose:** Counts the number of orders that did not breach the Service Level Agreement (25,628).
- **Logic:** Counts all rows where the SLA_Breach flag is 0 (False).

### Average Delivery Time
- **Formula:** `=AVERAGE(Data[Delivery_Time])`
- **Purpose:** Calculates the mean delivery time across all orders (71 minutes).

### Refund Rate %
- **Formula:** `=SUM(Data[Refund_Flag]) / [Total Orders]`
- **Purpose:** Calculates the percentage of orders that resulted in a refund.

### Delay Stage Contribution (Donut Chart)
- **Formula:** `=SUMIFS(Data[Delay_Count], Data[Delay_Stage], "Delivery") / SUM(Data[Delay_Count])`
- **Purpose:** Calculates the 53.85% contribution of the "Delivery" stage to overall delays.

##  Advanced Data Lookups (If used)

### Dynamic Driver Performance (Using XLOOKUP)
- **Formula:** `=XLOOKUP([Selected_Driver], Data[Driver_Name], Data[Average_Delivery_Time])`
- **Purpose:** Powers the interactive "Driver Name" slicer in the top right corner, dynamically updating the charts based on user selection.
