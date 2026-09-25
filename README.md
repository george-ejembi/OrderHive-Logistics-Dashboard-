# OrderHive Logistics Performance Dashboard

![Overview Dashboard](images/overview_dashboard.png)
![Driver Analytics Dashboard](images/driver_analytics_dashboard.png)

## Project Overview
A logistics performance dashboard that identifies where bottlenecks hide and which top drivers outperform to fix what breaks and scale what works. This dashboard provides actionable insights into order volumes, revenue, delivery delays, and driver performance.

## Business Objectives
- Track overall order volume, gross/net revenue, and on-time delivery rates.
- Identify operational pressure peaks and their impact on delivery times.
- Analyze the root causes of delivery delays (Restaurant, Order Processing, or Delivery).
- Evaluate individual driver performance based on SLA breaches, refund rates, and delivery times.

## Tech Stack
- **Data Visualization:** Power BI (or Tableau)
- **Data Transformation:** Power Query / DAX
- **Data Source:** *(e.g., SQL, Excel, Mock Data)*

## Dashboard Features & Key Insights

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

## Repository Structure
- `/dashboard`: Contains the main BI project file.
- `/data`: Contains sample/mock data or data dictionaries.
- `/docs`: Contains detailed business insights and data definitions.
- `/images`: Contains screenshots used in this README.

##  How to Use
1. Clone the repository: `git clone https://github.com/YourUsername/OrderHive-Logistics-Dashboard.git`
2. Open the `.pbix` file in Power BI Desktop.
3. Refresh the data source (if connected to a local dataset) or explore the pre-loaded data model.

## Author
**George E.** | Rock Quant Analytical Consult
- LinkedIn: [linkedin.com/in/george-ejembi-8489bb273]
