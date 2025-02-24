<h1 align='center> Cyclistic Bike-Share Analysis: Unlocking Rider Behavior Patterns 🚴♂️📊 </h1>


# Project Overview

This R-based case study analyzes Cyclistic's bike-share data (Q1 2019 & Q1 2020) to compare usage patterns between **members** (annual subscribers) and **casual** riders. Discover actionable insights to drive data-informed marketing strategies!

# Key Steps in Analysis

## 🛠️ Data Preparation:

* Data Loading & Exploration

* Imported datasets with inconsistent column names (e.g., `trip_id` vs. `ride_id`).

* Standardized column names across years for seamless merging.

## Data Cleaning:

* Removed non-essential columns (`start_lat`, `end_lat`, `gender`, `birthyear`) due to high missing values.

* Filtered out invalid records:

  Rides with negative/zero durations

  Maintenance-related rides (`HQ QR` stations)

## Feature Engineering:

* Converted datetime strings (`started_at`, `ended_at`) to POSIXct format.

* Created time-based features: `month`, `day`, `year`, `day_of_week`.

* Calculated `ride_length` (seconds) to quantify trip durations.

## Outlier Handling:

* Used boxplots and Q-Q plots to identify skewed distributions in ride durations.

# 🧐 Key Insights:

* **Temporal Patterns:** Weekday vs. weekend usage trends, seasonal variations.

* **Ride Duration:** Members vs. casual riders’ average trip lengths.

* **Station Popularity:** Most frequent start/end stations for each group.


# 🔮 Future Work:

* **Expand Timeframe:** Analyze multi-year data for long-term trends.

* **Geospatial Analysis:** Map popular routes using latitude/longitude data (excluded in this iteration).

* **Weather Integration:** Correlate ridership with weather conditions.

* **Customer Segmentation:** Identify subgroups within casual riders for targeted campaigns.

* **Predictive Modeling:** Forecast demand to optimize bike redistribution.


# ⚙️ Technical Setup:

* **Language:** R

* **Libraries:** `tidyverse`, `lubridate`, `conflicted`

* **Environment:** Ensure R kernel is configured before running the notebook.


# 💡 Why This Matters:

By understanding how members and casual riders differ, Cyclistic can design tailored marketing strategies to convert casual users into loyal subscribers, driving revenue growth.


Ready to explore? Dive into the R notebook to see the code, visualizations, and detailed findings! 📈🔍

(Note: Ensure datasets `Divvy_Trips_2019_Q1.csv` and `Divvy_Trips_2020_Q1.csv` are placed in the `/content/` directory before execution.)
