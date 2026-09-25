# OrderHive Logistics Performance Dashboard (Microsoft Excel)

##  Project Overview
An advanced, interactive Microsoft Excel dashboard built to identify operational bottlenecks, track financial metrics, and analyze driver efficiency for OrderHive Logistics. The project transforms raw operational data into a dynamic dark-mode UI to help management "fix what breaks and scale what works."

##  Business Objectives
- Track overall order volume, gross/net revenue, and on-time delivery rates.
- Identify operational pressure peaks and their impact on delivery times.
- Analyze the root causes of delivery delays (Restaurant, Order Processing, or Delivery).
- Evaluate individual driver performance based on SLA breaches, refund rates, and delivery times.

##  Tech Stack & Excel Skills Used
- **Data Transformation:** Power Query, Advanced Formulas (`XLOOKUP`, `INDEX/MATCH`, `SUMIFS`, `IFERROR`).
- **Data Analysis:** Dynamic PivotTables, PivotCharts, Calculated Fields.
- **UI/UX & Interactivity:** Form Control Slicers, Timeline filters, Conditional Formatting, Custom Chart Templates, Shape Layering for KPI cards.
- **Dashboard Design:** Custom dark-mode theme, gridline removal, and dynamic text boxes for automated annotations.

##  Dashboard Features & Key Insights

### Page 1: Executive Overview
- **KPIs:** 72.32K Total Orders, $6.78M Gross Revenue, 25,628 On-Time Orders.
- **Operational Pressure:** Identified a midday pressure peak (Hours 12-14). The data suggests this is a process failure rather than a demand overload, as order volume drops but delivery times spike.
- **Delivery Delays:** The "Delivery" stage is the largest contributor to delays (53.85%), followed by Restaurant Processing (30.77%) and Order Processing (15.38%).
- **End-to-End Delivery:** Average delivery time increased from 57 minutes in January to 91 minutes in April.

### Page 2: Driver & Area Analytics
- **Delivery Areas:** Performance is evenly split across Fremont (33%), Hayward (33%), and Union City (34%).
- **Average Times:** Average Delivery Time is 71 minutes, with Restaurant Processing taking 40 minutes and Order Processing taking 20 minutes.
- **Driver Performance:** Analyzed drivers (Audrey, Gail, Helen, etc.) by average delivery time, refund rates, and tip service fees. 
- **SLA Insights:** High SLA breach almost always drives a high refund rate, but not perfectly, indicating that driver behavior and strategies matter.

##  How to Use
1. Clone the repository or download the `.xlsx` file from the `/dashboard` folder.
2. Open the file in Microsoft Excel (Excel 2016 or later recommended).
3. If prompted, enable editing and macros (if applicable).
4. Use the "Driver Name" slicer in the top right corner to filter the entire dashboard dynamically.

##  Author
**George E.** | Rock Quant Analytical Consult
- LinkedIn: linkedin.com/in/george-ejembi-8489bb273
