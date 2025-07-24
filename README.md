# 🚦 UK Road Accident Analysis Dashboard

This project presents a comprehensive data-driven analysis of road accidents across the United Kingdom using Power BI. The dashboard is designed to uncover key insights into accident severity, environmental conditions, road infrastructure, and vehicle involvement — enabling stakeholders to make informed decisions for improving public safety and reducing traffic-related casualties.

## 📌 Project Objective

The primary goal of this project is to analyze UK road accident data to:
- Understand when, where, and under what conditions accidents occur
- Identify high-risk areas such as specific road types, junction controls, or weather conditions
- Reveal patterns in accident severity and vehicle involvement
- Provide actionable insights and policy recommendations to improve road safety

## 🧰 Tools and Technologies

- **Power BI**: For data modeling, DAX calculations, and dashboard creation
- **DAX (Data Analysis Expressions)**: To create KPIs and custom measures
- **Excel / CSV**: Original dataset provided in structured format
- **GitHub**: For version control and sharing

## 📚 Dataset

The dataset used in this project is publicly available on Kaggle:

🔗 [Road Traffic Accident Data – United Kingdom](https://www.kaggle.com/datasets/atharvasoundankar/road-accidents-dataset)

## 🗂️ Dataset Description

The dataset includes features such as:
- `Accident_Index`, `Accident Date`, `Time`, `Day_of_Week`
- `Road_Type`, `Junction_Control`, `Accident_Severity`
- `Number_of_Casualties`, `Number_of_Vehicles`
- `Weather_Conditions`, `Light_Conditions`, `Road_Surface_Conditions`
- `Vehicle_Type`, `Urban_or_Rural_Area`, and geographic coordinates

No missing values were present in the dataset. Minor cleaning was done to correct typos in categorical variables (e.g., “Fetal” to “Fatal”).

## 🧹 Data Cleaning

- Corrected typos such as “Fetal” → “Fatal” and “Auto traffic sigl” → “Auto traffic signal”
- Verified that there were no missing values
- Standardized categorical entries for consistency

## 🧠 Data Modeling & DAX

- Created a separate `Calendar` table using `CALENDAR` function
- Linked the `Calendar` table to the accident data to support time-based analysis
- Developed custom DAX measures:
  - `Total Accidents`
  - `Total Casualties`
  - `Total Vehicles`
  - `Fatal %`, `Serious %`, `Slight %`

## 📊 Dashboard Structure

Due to the breadth of insights, the dashboard was split into two separate pages:

### 📍 Page 1: Accident Trends & Conditions Overview

![image alt](https://github.com/srinibas-masanta/Road-Accident-Analysis-Dashboard/blob/32010b575056267d48e6563e7b619d7d53014b21/Dashboard%20Screenshots/Page%201.png)  

This page focuses on when accidents happen and under what environmental conditions. It includes:
- KPIs for Total Accidents, Casualties, Vehicles, and Severity Breakdown
- Line chart: Accidents over Time
- Stacked bar charts for Road Surface Conditions and Weather Impact
- Column chart for Day of the Week distribution
- Multi-row card showing Casualties by Vehicle Type
- Slicers: Urban/Rural and Light Conditions

**Key Insights:**
- Most accidents happen in good weather and daylight, indicating behavioral causes
- Fridays record the highest number of accidents
- Cars dominate casualty figures, followed by bikes and goods vehicles

### 🏙️ Page 2: Location & Infrastructure Impact

![Image Alt](https://github.com/srinibas-masanta/Road-Accident-Analysis-Dashboard/blob/32010b575056267d48e6563e7b619d7d53014b21/Dashboard%20Screenshots/Page%202.png)

This page examines how location and road design influence accident patterns. It includes:
- KPIs for Total Accidents, Casualties, Vehicles, and Severity Breakdown
- Column chart: Top Junction Controls
- Bar chart: Road Type Distribution
- Pie and Donut charts for Light Conditions and Urban/Rural split
- Map: Casualties by Location (Latitude/Longitude)
- Slicers: Day of Week and Vehicle Type

**Key Insights:**
- Uncontrolled junctions are the leading contributors to accidents
- Urban areas account for ~65% of total accidents
- Single carriageways show the highest accident frequency
- Regional hotspots like London, Birmingham, and Manchester show dense clusters

## ✅ KPI Summary

| KPI                    | Value      |
|------------------------|------------|
| Total Accidents        | 308K       |
| Total Casualties       | 418K       |
| Total Vehicles         | 563K       |
| Fatal Casualties %     | 1.3%       |
| Serious Casualties %   | 13.2%      |
| Slight Casualties %    | 85.5%      |

## 🧾 Recommendations

1. **Improve Data Collection**: High volume of missing values in junction controls shows a need for better data capture.
2. **Target Unsafe Junctions**: Focus on redesigning uncontrolled junctions with better signage and signals.
3. **Enhance Urban Infrastructure**: Prioritize improvements in high-traffic urban zones and introduce smart signaling.
4. **Address Behavioral Risks**: Awareness campaigns should target driving behavior during good conditions.
5. **Prioritize High-Risk Vehicles**: Special focus on bikes and goods vehicles in safety policies.
6. **Use Geographic Targeting**: Direct safety resources to regional hotspots identified on the map.

## 📌 Conclusion

This dashboard goes beyond visualization. It acts as a decision-support tool for policymakers, urban planners, and traffic safety analysts. It uncovers critical accident patterns, highlights areas for infrastructure and behavioral improvement, and provides a roadmap for reducing road-related fatalities and injuries.
