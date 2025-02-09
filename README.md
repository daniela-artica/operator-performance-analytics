# Identification of inefficient operators for a telecommunications company

## Project Background

This project analyzes operator efficiency in a telecommunications company that provides virtual phone services. The goal is to identify inefficient operators based on key performance metrics. The insights from this analysis will help supervisors monitor operator performance and optimize call handling.

The company considers an operator inefficient if they:
- Have a high number of missed incoming calls.
- Have long wait times for incoming calls.
- Make significantly fewer outbound calls (if expected to do so).

## Executive Summary

- Two datasets containing operator call activity were analyzed to assess efficiency.
- The primary inefficiency indicators were missed incoming calls, wait times, and outbound call volume.
- Out of the total operators analyzed, **15 operators** were identified as inefficient based on these criteria.
- Histograms were used to visualize the distribution of wait times, missed calls, and outbound call volume.
- A **t-test** was conducted to compare wait times between efficient and inefficient operators, revealing a statistically significant difference (p-value < 0.05).
- A cluster analysis using **k-means** identified distinct groups of operators based on their efficiency scores.
- The findings suggest actionable recommendations to improve call handling efficiency.

## Key Insights

- Operators with the highest missed call rates also had the longest wait times, indicating a correlation between these two inefficiency factors.
- **15 operators** were classified as inefficient based on their performance metrics.
- The histogram analysis showed that inefficient operators had wait times skewed towards higher values, while efficient operators had a more balanced distribution.
- Outbound call volume analysis revealed that some operators, despite handling outbound calls, made significantly fewer calls than expected.
- A **t-test** confirmed that inefficient operators had a significantly higher average wait time compared to efficient ones.


## Recommendations

- Implement targeted training programs for operators with high wait times and missed calls.
- Adjust workload distribution to ensure fair call handling among operators.
- Introduce automated alerts for supervisors when an operator’s inefficiency crosses a threshold.
- Encourage the use of best practices observed in high-performing operator clusters.
- Conduct periodic statistical analysis to continuously monitor operator performance and detect emerging inefficiency trends.