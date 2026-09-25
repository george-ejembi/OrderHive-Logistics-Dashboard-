# Data Transformation & ETL (Power Query)

Before building the dashboard, raw data was cleaned and transformed using Excel's Power Query. Below are the key steps taken:

1. **Data Extraction:** Imported raw CSV/Excel data containing order logs.
2. **Data Type Formatting:** Ensured dates were formatted as DateTime and financial columns as Decimal Numbers.
3. **Handling Missing Values:** Replaced null values in the `Driver_Tip` column with 0.
4. **Calculated Columns:** Created a custom column `Order_Hour` using `Time.Hour([Order_Time])` to analyze operational pressure peaks by hour (0-23).
5. **Merging Tables:** Merged the `Orders` table with the `Drivers` table using `Driver_ID` to bring in driver names and regional data (Fremont, Hayward, Union City).
6. **Unpivoting:** Unpivoted the delay stage columns (Order Processing, Restaurant Processing, Delivery) into a single `Delay_Stage` column to create the donut chart visualization.
