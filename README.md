# AtliQ Grands | Hotel Performance & Booking Analysis

## Project Overview

AtliQ Grands is a five-star hotel chain operating across multiple cities in India. The company has been experiencing a decline in revenue and market share due to increasing competition and ineffective management decisions.

The objective of this project is to explore hotel performance data, identify patterns affecting revenue and bookings, and provide data-driven insights that can support better business decisions.

This project covers data modeling, exploratory data analysis (EDA), interactive dashboard development, and business recommendations.

## Business Objectives

- Analyze revenue performance across different months, cities, and properties.
- Evaluate key hotel performance indicators such as ADR, Occupancy, and RevPAR.
- Understand booking behavior and booking status distribution.
- Analyze booking platforms based on revenue, cancellations, and no-shows.
- Identify potential areas for improvement and further investigation.

## Dataset

The project uses five CSV files:

| Table | Description |
|---|---|
| `dim_date` | Date information, including month and day type. |
| `dim_hotels` | Hotel details, including property name, city, and category. |
| `dim_rooms` | Room information and room categories. |
| `fact_bookings` | Booking-level information, including booking status, platform, revenue, and guest details. |
| `fact_aggregated_bookings` | Aggregated booking information, including capacity and successful bookings. |

The dataset covers May, June, and July.

## Tools & Technologies

- **Microsoft Excel:** Data exploration, PivotTables, and initial analysis.
- **Power Pivot:** Data modeling and DAX measures.
- **Power BI:** Interactive dashboard development and data visualization.

## Data Modeling

A data model was created using the five available tables:

- Two fact tables: `fact_bookings` and `fact_aggregated_bookings`.
- Three dimension tables: `dim_date`, `dim_hotels`, and `dim_rooms`.

The model connects booking and aggregated performance data with the relevant date, hotel, and room dimensions to support analysis across different business perspectives.

## Key Performance Indicators (KPIs)

The analysis focuses on the following metrics:

- **Total Revenue:** Revenue realized from hotel bookings.
- **ADR (Average Daily Rate):** Average revenue earned per occupied room.
- **Occupancy %:** Percentage of available rooms that were occupied.
- **RevPAR (Revenue per Available Room):** Revenue generated per available room.
- **Realisation %:** Revenue realized compared with revenue generated.
- **Total Bookings:** Total number of recorded bookings.
- **Successful Bookings:** Number of successful bookings based on the aggregated bookings table.
- **Cancellation Rate:** Percentage of bookings that were cancelled.
- **No-Show Rate:** Percentage of bookings where guests did not show up.

## Exploratory Data Analysis (EDA)

Excel PivotTables were used to investigate the data and explore several business questions.

### 1. Monthly Revenue Analysis

- Revenue decreased by approximately 4.8% in June compared to May.
- Revenue recovered by approximately 3.4% in July.
- July revenue remained slightly below May's level.
- June also recorded fewer checked-out bookings, while cancellations and no-shows decreased.

**Insight:** The decline in June cannot be explained by an increase in cancellation volume alone. Further analysis at the property and segment levels is needed.

### 2. Weekday vs. Weekend Analysis

- Weekdays generated approximately 1.07 billion in realized revenue.
- Weekends generated approximately 639 million.

**Insight:** Weekdays contributed more to total revenue. However, since there are more weekdays than weekend days, average revenue per day is required for a fair comparison.

### 3. City Performance Analysis

- Mumbai recorded the highest revenue contribution.
- Bangalore ranked second, followed by Hyderabad and Delhi.

**Insight:** Revenue is concentrated more heavily in Mumbai, but total revenue alone does not indicate which city has the highest profitability or operational efficiency.

### 4. Property Performance Analysis

- AtliQ Exotica recorded the highest property revenue.
- AtliQ Seasons recorded the lowest property revenue.
- AtliQ Seasons also showed the highest ADR and lowest occupancy among the properties.

**Insight:** AtliQ Seasons requires further investigation into its pricing strategy and demand patterns. Its lower total revenue may also be influenced by having only one property.

### 5. ADR & Occupancy Analysis

An approximately -86% correlation was observed between ADR and Occupancy across the properties.

**Insight:** The analysis indicates a negative relationship between room prices and occupancy in the observed data. However, correlation does not establish causation.

### 6. Booking Status Analysis

Across 134,590 recorded bookings:

- Checked Out: 94,411 bookings (approximately 70.2%).
- Cancelled: 33,420 bookings (approximately 24.8%).
- No Show: 6,759 bookings (approximately 5.0%).

**Insight:** Cancellations represent a considerable share of recorded bookings and should be monitored as part of booking performance analysis.

### 7. Booking Platform Analysis

- The "Others" category recorded the highest revenue.
- It also recorded the highest number of cancellations and no-shows.

**Insight:** Booking volume and total revenue are not sufficient to evaluate platform effectiveness. Cancellation rates, no-show rates, booking value, and acquisition costs should also be considered.

## Power BI Dashboard

The interactive dashboard consists of three main pages:

### 1. Executive Overview
Provides a high-level summary of hotel performance, including:
- Total Revenue
- ADR
- Realisation %
- Occupancy %
- RevPAR
- Total Successful Bookings
- Monthly Revenue Trend

### 2. Property Performance
Compares hotel properties based on:
- Total Revenue
- Occupancy %
- ADR
- RevPAR
- Relationship between ADR and Occupancy

### 3. Booking Analysis
Explores:
- Total Bookings
- Successful Bookings
- Cancellation %
- No-Show %
- Booking Status by Month
- Cancellations by Booking Platform
- No-Shows by Booking Platform

Interactive slicers allow users to filter the analysis by property, city, and month.

## Business Recommendations

Based on the findings, the following areas are recommended for further investigation:

1. **Review Pricing and Demand:** Investigate AtliQ Seasons' pricing strategy and demand patterns before making pricing adjustments.

2. **Investigate the June Revenue Decline:** Analyze performance by property, city, room category, and booking platform to identify the main contributors.

3. **Optimize Booking Channels:** Compare cancellation and no-show rates across platforms rather than relying on absolute counts.

4. **Evaluate Expansion Opportunities:** Assess market demand, competitor performance, available capacity, and expansion costs before making investment decisions.

5. **Improve Performance Monitoring:** Track Revenue, ADR, Occupancy, and RevPAR together to obtain a more complete view of hotel performance.

## Conclusion

This project demonstrates how raw hotel booking data can be transformed into meaningful business insights through data modeling, exploratory analysis, and interactive visualization.

The analysis highlights revenue trends, differences in property and city performance, booking behavior, and potential areas for operational improvement.

The final dashboard provides a consolidated view of hotel performance to support data-informed discussions and further business investigation.
