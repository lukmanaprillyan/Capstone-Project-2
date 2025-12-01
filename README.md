This project analyzes New York City taxi trip data to uncover customer demand patterns, trip characteristics, mobility performance, and behavioral insights across boroughs.
The goal is to answer the key problem statement:
How can taxi demand patterns across boroughs such as Manhattan, Brooklyn, Queens, the Bronx, and Staten Island help optimize fleet distribution and improve service performance?
This analysis includes data cleaning, preprocessing, feature engineering, exploratory data analysis (EDA), and visualization to build meaningful insights for mobility optimization and operational planning.

Several preprocessing and engineering steps were applied to refine the raw dataset:
Data Formatting
Converted timestamps, distance fields, speed values, and trip metrics into unified formats.
Standardized column naming for consistency.
Data Cleaning
Removed invalid records and missing values.
Processed distance and duration anomalies.
Removed outlier trips exceeding 80 miles to prevent skewed results.
Feature Engineering
Created trip_duration_min from dropoff_datetime – pickup_datetime.
Calculated avg_speed_mph using distance and duration.
Categorized distance into labels such as Very Short, Short, Medium, Long, Very Long.
Extracted pickup hour (0–23).
Generated borough-level aggregations and behavioral segments.

--- Exploratory Data Analysis ---

1. Demand Analysis
Trip volume by hour (0–23) across all boroughs.
Peak demand during 07–10 AM and 03–06 PM.
Manhattan shows consistently dominant ridership.
2. Borough-Level Insights
Geographic distribution of total trips.
Borough comparison based on distance category, average distance, and trip count.
3. Trip Characteristics
Distribution of categorized trip distances.
Average trip duration and speed across boroughs.
Mobility performance patterns that differ between urban and suburban zones.
4. Payment Method Analysis
Donut chart visualizing payment method proportions.
Card payments dominate, followed by cash and wallet-based payments.
5. Pickup Zone Insights
Identification of top pickup zones with longest average distances.
Dynamic Top-N filtering to adjust ranking interactively.

The analysis reveals clear customer demand patterns and trip behaviors across NYC boroughs, enabling:

- Better fleet allocation during high-demand periods
- Improved service quality and operational efficiency
- More targeted route planning and pricing strategies
- Stronger understanding of mobility behavior for decision-makers
- This project demonstrates how data-driven insights can enhance transportation services in a complex urban mobility ecosystem.

You can view the interactive Tableau dashboard here: 
https://public.tableau.com/views/NYVTLCTripDemandMobilityInsightsDashboard/Dashboard1?:language=en-GB&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link
