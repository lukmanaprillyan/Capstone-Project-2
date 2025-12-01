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
