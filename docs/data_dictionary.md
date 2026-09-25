# Data Dictionary: OrderHive Logistics Dataset

This document outlines the structure, data types, and descriptions of the fields used to build the OrderHive Logistics Performance Dashboard in Excel.

##  Order & Customer Details

| Field Name | Data Type | Description | Example |
| :--- | :--- | :--- | :--- |
| `Order_ID` | String | Unique identifier for each order. | ORD-84729 |
| `Order_Date` | DateTime | The date and timestamp when the order was placed. | 2024-01-15 12:30:00 |
| `Delivery_Date` | DateTime | The date and timestamp when the order was delivered. | 2024-01-15 13:45:00 |
| `Delivery_Area` | String | The geographical zone where the order was delivered. | Fremont, Hayward, Union City |

##  Driver Information

| Field Name | Data Type | Description | Example |
| :--- | :--- | :--- | :--- |
| `Driver_Name` | String | Name of the driver assigned to the delivery. | Aaron, Audrey, Kristina |
| `Driver_Tip` | Decimal | The tip amount received by the driver for the delivery. | $9.57 |

##  Financial Metrics

| Field Name | Data Type | Description | Example |
| :--- | :--- | :--- | :--- |
| `Gross_Revenue` | Decimal | Total revenue generated from the order before any deductions. | $6,786,304 |
| `Net_Revenue` | Decimal | Revenue after deducting refunds, fees, and costs. | $329.51K |
| `Refund_Flag` | Boolean | Indicates whether the order was refunded (1 = Yes, 0 = No). | 1 |
| `Refund_Rate` | Decimal | The percentage of orders refunded. | 4.5% |

##  Time & Operations Metrics

| Field Name | Data Type | Description | Example |
| :--- | :--- | :--- | :--- |
| `Order_Processing_Time` | Integer | Time taken (in minutes) to process the order internally. | 20 |
| `Restaurant_Processing_Time`| Integer | Time taken (in minutes) by the restaurant to prepare the food. | 40 |
| `Delivery_Time` | Integer | Total end-to-end delivery time (in minutes). | 71 |
| `SLA_Breach` | Boolean | Indicates if the delivery breached the Service Level Agreement (1 = Yes, 0 = No). | 0 |
| `Delay_Stage` | String | The specific stage where the delay occurred. | Delivery, Order Processing, Restaurant Processing |
| `Order_Hour` | Integer | The hour of the day the order was placed (0-23). | 14 |
