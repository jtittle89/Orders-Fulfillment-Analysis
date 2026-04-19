# Orders-Fulfillment-Analysis

Fulfillment Order Analytics Dashboard
Project Overview

This project analyzes a simulated distribution and fulfillment order dataset to evaluate vendor performance, order delays, and operational efficiency across distribution centers. The analysis was conducted using Excel for exploratory data analysis and Power BI for data visualization and dashboard reporting.

The goal of the project is to demonstrate how data analytics can improve order visibility, vendor performance monitoring, and supply chain decision-making within a purchase-to-pay workflow.

Business Problem

Distribution and fulfillment operations depend on vendors delivering materials on time so inventory is available when needed. Delayed shipments can cause inventory shortages, operational delays, and reduced customer satisfaction.

This project analyzes order lifecycle data to answer the following questions:

    What percentage of orders are delivered late?
    
    Which vendors have the highest delay rates?
    
    Which distribution centers handle the largest order volume?
    
    How does order lead time change over time?
    
    Where can operational visibility be improved?

Tools Used:

    Excel – Data exploration, pivot tables, and preliminary analysis
    
    Microsoft Power BI – Data modeling, DAX measures, and dashboard creation
    
    DAX – KPI calculations and analytical measures

Dataset

The dataset simulates purchase orders moving through a distribution network and contains:

    Vendor information
    Order lifecycle dates
    Distribution center locations
    Order quantities and values
    Shipment status and lead times


Excel Analysis

Initial analysis was performed in Excel to explore patterns in vendor performance and order fulfillment.

Key Excel Techniques:

    Pivot Tables
    Conditional Formatting
    Data filtering and sorting
    Calculated columns for shipment delays
    Shipment Delay Calculation

Shipment delay was calculated by comparing:

Actual Ship Date – Expected Ship Date

This allowed identification of late orders and vendor reliability.

Vendor Performance Analysis

Pivot tables were used to evaluate vendor performance metrics:

    Total orders per vendor
    Average lead time
    Number of late shipments
    Total order value

This analysis helped identify suppliers contributing to shipment delays.

Distribution Center Workload

Another pivot table was used to analyze order distribution across fulfillment locations.

Metrics analyzed:

    Total orders processed
    Total inventory value received
    Average lead time per location

This provides insight into operational demand across distribution centers.

Power BI Dashboard

An interactive dashboard was created in Power BI to visualize fulfillment performance and provide operational insights.

The dashboard focuses on improving order visibility and vendor performance monitoring.

Key Performance Indicators (KPIs)

The dashboard includes several core supply chain metrics:

    Total Orders
    Total Order Value
    Average Lead Time
    Late Order Percentage
    Late Order Percentage (DAX)
    Late Order % =
    DIVIDE(
        CALCULATE(COUNT(Orders[Order_ID]), Orders[Order_Status] = "Late"),
        COUNT(Orders[Order_ID]),
        0
    )

This metric measures the percentage of orders shipped later than the expected ship date.

Dashboard Visualizations

The Power BI dashboard includes the following visuals:

<img width="1395" height="795" alt="image" src="https://github.com/user-attachments/assets/814ca57c-6c51-4473-81c5-f4b12ce281bc" />


KPI Cards

    High-level metrics showing:
    
    Total Orders
    Total Order Value
    Late Order %
    Average Lead Time
    
    These provide a quick snapshot of fulfillment performance.

Vendor Delay Analysis

A bar chart displays the number of late shipments by vendor.

    Purpose:
    
    Identify suppliers contributing to delivery delays
    Support vendor performance management

Distribution Center Order Value

A bar chart showing total order value by distribution center.

    Purpose:
    
    Understand operational demand
    Identify high-volume locations

Order Status Breakdown

A donut chart showing order status distribution:

    On Time
    Late
    Delivered
    In Transit
    
    Purpose:
    
    Provide quick visibility into order fulfillment performance.

Lead Time Trend

A line chart showing average lead time over time.
    
    Purpose:
    
    Track fulfillment efficiency
    Identify trends in vendor performance.
    Key Insights

The analysis demonstrates several operational insights:

Vendor performance varies significantly, with some suppliers contributing disproportionately to late shipments.
Certain distribution centers process higher order volumes and inventory value.
Shipment delays directly impact overall lead time and order fulfillment performance.

Tracking these metrics helps organizations improve supply chain reliability and operational efficiency.

Skills Demonstrated

This project highlights several analytical skills relevant to fulfillment and operations roles:

    Data exploration and transformation
    Supply chain KPI analysis
    Vendor performance monitoring
    Excel data analysis
    Dashboard development
    DAX calculations
    Data visualization for operational insights
