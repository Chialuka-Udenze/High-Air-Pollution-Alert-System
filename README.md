# High-Air-Pollution-Alert-System
The goal of this project is to create a tool that allows Canadian healthcare professionals to easily interpret and analyze crucial environmental factors that contribute to air pollution and alert channels necessary for improving healthcare decision-making processes and patient outcomes.
The project will focus on creating intuitive visualizations, ensuring data accuracy, and maintaining actionable insights
## DELIVERABLES
- A fully functional prototype of the healthcare data visualization dashboard.
- An analysis of the most efficient channels to alert local residents on high concentration of Air pollutants.
- Data visualizations of the concentration of air-based carcinogens in different areas

## Data Sets - STATSCAN
- Global Air Pollution Dataset
- Lung Cancer Dataset

## 1.Feature Engineering & Data Cleaning (Using Python)
🔹 Global Air Pollution Dataset:
  - Converted AQI columns from text to numeric
  - Normalized city name formats
  - Standardized AQI category labels
  - Verified no duplicates

🔹 Lung Cancer Dataset:
  - Dropped irrelevant columns (e.g., DGUID, VECTOR)
  - Removed trailing spaces in column names
  - Renamed key fields (REF_DATE → Year, VALUE → Value)
  - No missing values in critical columns

| Derived Variable | Function|
|---|---|
|Average AQI (Air Quality Index) |Long-term exposure per city|
|Pollution Index | Combined score from PM2.5, NO₂, CO, Ozone |
| High-Pollution % | % days AQI > 100|
|Yearly AQI Change | Tracks Annual trends|
|Dominant Pollutant | Top daily AQI contributor|
|Pollutant Ratio | NO₂ to PM2.5 | 
|Severity Level | Categorizes AQI (e.g., Good, Unhealthy) | 
|Stage Index | Measures cancer severity|
|Survival Rate | % alive after 1–5 years |
| Pollution-Cancer Risk | Combines AQI & incidence |
| Gender Risk Gap | Male vs. Female comparison | 
| Mortality by Region |  Death % across areas | 

## 2. Dashboard Building (Using Power BI)
- Created an interactive slicer to display the average NO2, PM2.5, Ozone and CO across Canada and different countries in the world
- Included correlation scatter plots to show the relationship between NO2, PM2.5, Ozone and CO and Air Quality Index (AQI).
- Highlighted the count of Lung Cancer (Categorized by Stage 1 to 4) across different provinces in Canada 
- Showed the % usage of digital marketing across healthcare, education and real estate sectors to show the most effective channel to communicate with local residents against the chances of getting Lung cancer if they reside in areas with high percentage of air-based carcinogens



