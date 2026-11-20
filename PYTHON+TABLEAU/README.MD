## EV Adoption and Air Quality Analysis in India

## Project Overview

This project explores the relationship between Electric Vehicle (EV) adoption and air quality across different states in India. Using vehicle registration and Air Quality Index (AQI) datasets, the analysis identifies the top five states with the highest EV adoption and examines whether these states experience better air quality compared to states with lower EV adoption.

The project uses **Tableau** to transform raw data into interactive visualizations and dashboards, helping uncover patterns and relationships between EV adoption and air pollution.

## Objectives

- Identify the top five Indian states with the highest EV adoption.
- Calculate and compare EV adoption percentages across states.
- Analyse average AQI levels in states with high and low EV adoption.
- Explore the relationship between EV adoption and air quality.
- Present key findings through an interactive Tableau dashboard and story.

## Datasets Used

Two datasets were used for this analysis:

### 1. Electric Vehicle Registration Dataset
**File:** `cleaned_master-data-state-vehicle-class-and-fuel-type-wise-total-number-of-vehicles-registered-in-each-month-in-india.csv`

Contains vehicle registration information across Indian states.

Key columns:
- `year` – Year of registration
- `state` – Indian state
- `fuel` – Type of vehicle fuel
- `value` – Number of registered vehicles

### 2. Air Quality Index Dataset
**File:** `cleaned_day-wise-state-wise-air-quality-index-aqi-of-major-cities-and-towns-in-india.csv`

Contains air quality information for major cities and towns across Indian states.

Key columns:
- `state` – Indian state
- `date` – Date of AQI measurement
- `area` – City or town
- `prominent_pollutants` – Major pollutants recorded
- `aqi_value` – Air Quality Index value

## Tools and Technologies

- **Tableau** – Data visualization, dashboard creation and storytelling
- **CSV** – Dataset format
- **Python** – Handling duplicate observations and preparing data for analysis

## Methodology

### 1. Data Collection and Preparation
- Collected two datasets: Electric Vehicle Registration Data and Air Quality Index (AQI) Data.
- Used **Python (Pandas)** for data cleaning and preprocessing.
- Handled missing values, duplicate records, inconsistent formats and data type issues.
- Standardized relevant columns and prepared the datasets for analysis.
- Exported the cleaned datasets for visualization in Tableau.

### 2. EV Adoption Analysis
EV registrations were calculated by considering the following fuel categories:

- Electric (BOV)
- Pure EV
- Plug-in Hybrid EV

Strong Hybrid EV was excluded from the primary EV calculation because it does not generally require external charging.

The EV adoption percentage was calculated using:

`EV Adoption % = (EV Registrations / Total Vehicle Registrations) × 100`

States were ranked based on their EV adoption percentages to identify the top five states with the highest EV adoption.

### 3. AQI Analysis
- Used the cleaned AQI dataset to analyse air quality across Indian states.
- Applied Tableau Level of Detail (LOD) calculations to handle repeated AQI observations.
- Calculated average AQI at the area, date and state levels.
- Used state-wise average AQI values to evaluate air quality across different EV adoption groups.

The AQI dataset covers the overlapping analysis period of 2015–2025, while the vehicle registration dataset covers 2014–2025.

### 4. Comparative Analysis
States were divided into two categories:

- **High EV Adoption:** Top five states based on EV adoption percentage.
- **Low EV Adoption:** All remaining states.

The average AQI of both groups was compared to investigate whether states with higher EV adoption experience better air quality.

### 5. Data Visualization
- Used **Tableau** to create interactive visualizations and dashboards.
- Developed an EV adoption ranking chart.
- Created an average AQI comparison between high and low EV adoption states.
- Built a scatter plot with a trend line to explore the relationship between EV adoption and AQI.
- Combined the visualizations into an interactive dashboard and Tableau Story.
## Tableau Dashboard

The project includes three major visualizations:

### 1. EV Adoption Ranking
Displays the top five states with the highest EV adoption percentages and compares their adoption levels.

### 2. Average AQI: High vs Low EV Adoption
Compares the average AQI of states with high EV adoption against states with lower EV adoption.

### 3. EV Adoption vs AQI
A scatter plot showing the relationship between state-wise EV adoption percentages and average AQI values, including a trend line to identify the overall relationship.

## Key Insights

- EV adoption levels vary across Indian states.
- States with higher EV adoption do not necessarily have better air quality.
- Air quality is influenced by multiple factors, including industrial emissions, population density, traffic conditions and geographical factors.
- The relationship between EV adoption and AQI should be interpreted as an association rather than proof of causation.

## Project Outcome

An interactive Tableau dashboard and story were developed to present the findings in a clear and visually engaging manner.

The project demonstrates how data analytics and visualization can be used to explore the relationship between sustainable transportation and environmental quality.

## Conclusion

Electric vehicles have the potential to reduce transport-related emissions and contribute to cleaner urban environments. However, this analysis highlights that increased EV adoption alone may not be sufficient to ensure better air quality. A combination of cleaner transportation, industrial emission control and sustainable urban planning is essential for improving air quality across India.


**Skills Demonstrated:** Data Cleaning | Data Analysis | Tableau | Data Visualization | Dashboard Development | Exploratory Data Analysis | Environmental Data Analysis
