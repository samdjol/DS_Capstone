# DS Capstone Project
Road to Safety: Data-Driven Insights for US Traffic Accidents
Overview
This project analyzes a comprehensive dataset of U.S. traffic accidents to identify the key infrastructure and environmental factors that contribute to accident severity. The goal is to provide the Department of Transportation (DOT) with actionable, data-driven recommendations to enhance road safety and optimize emergency response.

Key Insights (BLUF)
Not all safety features are equal for preventing fatalities. While features like traffic signals and crossings are significantly associated with a lower percentage of fatal (Category 4) accidents, conventional controls like stop signs and roundabouts show no statistical impact on reducing the most severe incidents.

The most dangerous conditions are not always the most obvious. Darkness and snowy conditions show the most significant increase in the proportion of fatal accidents. Surprisingly, conditions like rain and fog are less associated with severe outcomes, likely due to heightened driver caution.

Junctions are critical hotspots for severe accidents. The presence of a junction is associated with a notable increase in the likelihood of a fatal accident, identifying these areas as prime targets for safety reviews and engineering improvements.

Business Problem
For the Department of Transportation (DOT), reducing traffic accidents is a critical mission that directly impacts public safety and economic costs. This analysis aims to move beyond general accident counts to identify the specific, high-impact factors that contribute to the most severe, life-threatening incidents. By understanding these root causes, the DOT can make more strategic investments in infrastructure, develop more effective safety policies, and improve emergency response protocols.

Data
This analysis utilizes the "US Accidents (2016-2023)" dataset, a country-wide traffic accident dataset covering 49 states of the USA. The data was collected from multiple traffic APIs and contains over 7.7 million records.

Source: Kaggle

File Used: US_Accidents_March23.csv

Methodology
The analysis was conducted using Python with the pandas, SciPy, and Matplotlib libraries. The core methodology involved:

Data Preparation: The raw dataset was cleaned and preprocessed. This included handling missing values, standardizing categorical data (e.g., creating Weather_Category and Light_Condition), and creating a binary target variable (is_severity_4) to isolate the most severe accidents.

Statistical Analysis: A Chi-Square Test of Independence was used to determine the statistical significance of the relationship between various road features (e.g., Junction, Stop, Traffic_Signal) and accident severity.

Insight Generation: By comparing the proportion of severe accidents under different conditions, we identified the factors with the most practical and impactful influence on accident outcomes.

Visualization: An interactive dashboard was created in Tableau to allow for dynamic exploration of these findings.

Initial exploration with machine learning models (Logistic Regression) was conducted, but the project's focus was strategically pivoted to statistical analysis to provide more direct and interpretable insights in line with the business objectives.

Key Findings & Recommendations
Recommendation 1: Prioritize High-Impact Safety Features for Fatality Prevention
Finding: Traffic signals and designated crossings are significantly associated with a lower percentage of fatal accidents, while stop signs and roundabouts are not.

Recommendation: The DOT should re-evaluate its safety budget allocation to prioritize the installation and maintenance of traffic signals and well-marked crossings in high-risk areas, as these have a proven impact on reducing the most severe accidents.

Recommendation 2: Launch a Targeted "Junction Safety Initiative"
Finding: The presence of a junction is associated with a more than 1% increase in the occurrence of Category 4 accidents, making them uniquely dangerous hotspots.

Recommendation: The DOT should launch a "Junction Safety Initiative" to conduct a systematic review of the most dangerous junctions and implement proven safety countermeasures, such as adding dedicated turning lanes or improving signal timing.

Recommendation 3: Implement a Dynamic Alert System for Emergency Services
Finding: Darkness and snowy conditions show the most significant increase in the proportion of fatal accidents.

Recommendation: The DOT should collaborate with emergency services to develop a dynamic, tiered alert system. This system would automatically elevate the readiness level of responders based on real-time weather and light data, ensuring resources are strategically allocated before an incident occurs.

Contact
Author: Samuel Jolinger
