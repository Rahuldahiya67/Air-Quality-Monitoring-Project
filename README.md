# Air Quality Monitoring Project: Detailed Report

## Introduction
Public health is directly impacted by air quality, one of the most important environmental factors. The goal of this project is to analyze and visualize real-time Air Quality Index (AQI) data across major Philippine cities using PySpark and Databricks. A data stream is simulated, window-based stream processing is implemented, detailed data analysis is done, and dynamic visualizations are made.

## Methodology
### 1. Streaming Data Simulation
- Static datasets for November and December 2023 were used to simulate real-time data.
- To resemble streaming behavior, a timestamp was added to every record.
- Used the DataFrame API in PySpark to manipulate data effectively.

### 2. Window-Based Stream Processing
- AQI data was aggregated at 1-hour intervals using window techniques.
- Computed trends across time, rolling averages, and Z-scores for anomaly detection.
- Utilizing the proper window requirements, late-arriving data issues were resolved.

### 3. In-Depth Data Analysis
- AQI distribution by city, trends, and anomalies were investigated.
- Long-term trends were found by using rolling averages.
- Abnormalities in real-time data were identified using Z-scores.
- By contrasting the present AQI values with the past data, trends were examined.

### 4. Innovative Visualization
- To visualize the AQI trend in real time, Matplotlib was used.
- For dynamic and interactive displays, make use of Databricks' visualization features.
- Included more graphics for more thorough insights, such as trend charts, box plots, and scatter plots.

## Strengths
- **Real-Time Study:** By enabling the study of AQI data in real-time, the technique enables prompt responses to changes in the environment.
- **Scalability:** PySpark with Databricks' combined use guarantees scalability for managing huge datasets and future growth.
- **Comprehensive Analysis:** The approach offers a comprehensive picture of air quality by taking into account a number of factors, such as distribution, trends, and anomalies.

## Weaknesses
- **Data Quality:** The quality of the supplied data has a significant impact on how effective the analysis is. Biased outcomes could arise from inaccurate source data.
- **Assumed Stationarity:** The study makes the assumption that the AQI data's underlying patterns are stationary. Prediction accuracy may be impacted by non-stationary trends.
- **Limited Historic Data:** Additional extensive datasets would enhance the precision of trend analysis, as the approach may be constrained by the previous data that is already accessible.

## Potential Real-World Impacts
- **Public Health Decision-Making:** Health authorities are empowered to make well-informed decisions to safeguard the public health by having real-time information about AQI trends and abnormalities.
- **Environmental Policy Development:** By spotting patterns and trends in air quality, the study can help create environmental policies that are both successful and sustainable.
- **Community Awareness:** By using dynamic visualizations, residents can become more aware of the problems with air quality and be more involved in local environmental projects.

## Conclusion
The project showcases the possibilities of real-time air quality analysis with PySpark and Databricks. Its scalability, thorough analytical methodology, and real-time capabilities are its strongest points. But it's important to take into account the constraints of assumed stationarity and solve issues with data quality. The project's practical effects include supporting community knowledge of sustainable environmental practices, influencing environmental policy, and assisting with public health decisions.
