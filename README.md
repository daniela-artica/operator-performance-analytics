# Identification of inefficient operators for a telecommunications company

## Project Background

This project analyzes operator efficiency in a telecommunications company that provides virtual phone services. The goal is to identify inefficient operators based on key performance metrics. The insights from this analysis will help supervisors monitor operator performance and optimize call handling.

The company considers an operator inefficient if they:
- Have a high number of missed incoming calls.
- Have long wait times for incoming calls.
- Make significantly fewer outbound calls (if expected to do so).

## Executive Summary

- Even though waiting times are relatively low, with an average of 60 seconds per call, 34% of call were missed. This results indicate potential areas of improvement in terms of operator efficiency.  
- Three types of operators were identified, and efficiency metrics were evaluated accordingly:
  **1. Operators handling both incoming and outgoing calls:** These operators do not show inefficiencies across all three metrics simultaneously, but 7 of them stand out negatively in one or two key metrics.
  **2. Operators handling only incoming calls:** Four inefficient operators were identified, as they rank in the top 25% for both missed calls and average wait time.
  **3. Operators handling only outgoing calls:** Four inefficient operators were identified, as they rank in the bottom 25% in terms of the number of outgoing calls.
-Correlation analysis showed that the call volume is a crucial factor that impacts an operator's efficiency. A high workload is closely linked to higher levels of inefficiency, suggesting that monitoring and managing workload are essential for optimizing operator efficiency.

- A **t-test** was conducted to compare wait times between efficient and inefficient operators, revealing a statistically significant difference (p-value < 0.05).
- A cluster analysis using **k-means** identified distinct groups of operators based on their efficiency scores.
- The findings suggest actionable recommendations to improve call handling efficiency.

## Key Insights

- **Correlation analysis:**
  1. A strong positive correlation was found between the number of calls handled by an operator and the wait time, implying that higher call volume may signal an increase of waiting times and, therefore, an operator's inefficiency. 
  2. There is a strong positive correlation between the number of calls handled and the total call duration, indicating that as the number of calls increases, the total duration also increases.
  3. A moderate positive correlation was observed between wait time and total call duration, suggesting that when total call duration is longer, wait times also tend to increase.
  4. Operators with the highest missed call rates also had the longest wait times, indicating a correlation between these two inefficiency factors.

- **Hypothesis testing:**
A series of hypothesis were tested to validate which factors affect operators performance the most.
  -  Hypothesis 1: There are significant differences in the average wait time between operators who handle both types of calls and those who handle only incoming calls.
  -  Hypothesis 2: There are significant differences in the number of missed calls between operators who handle both types of calls and those who handle only incoming calls.
  -  Hypothesis 3: There are significant differences in the number of outgoing calls between operators who handle both types of calls and those who handle only outgoing calls.
  -  Hypothesis 4: There is a significant relationship between the total number of calls handled by an operator and the number of missed calls.
  -  Hypothesis 5: There is a significant relationship between the total number of calls handled by an operator and the wait time for calls.

**Hypothesis 1, 2 and 3: Rejected** 
The operators' work mode does not affect their efficiency in terms of the number of missed calls, wait time, or the number of outgoing calls made.

**Hypothesis 4: Confirmed**
With a correlation of 0.4, it can be concluded that there is a moderate positive correlation between the total number of calls handled and the number of missed calls. In other words, as an operator's workload increases, the number of missed calls also rises, leading to greater inefficiency.

**Hypothesis 5: Confirmed**
The Pearson correlation value of 0.86 indicates a very strong positive linear relationship between workload and an operator's wait time. As the operator receives more calls, the wait time also increases, leading to greater inefficiency.

## Recommendations

- Since inefficiency is strongly linked to operator workload, it is recommended to redistribute calls more evenly among operators to prevent overload. Implementing an intelligent call distribution system could improve wait times and reduce the number of missed calls.

- Although the work mode does not directly affect efficiency, it is advisable to continue monitoring key metrics (missed calls, wait time, and outgoing calls) to detect any signs of inefficiency early.

- Reviewing the workflow to enhance operator efficiency is also recommended, with a focus on reducing wait times without compromising service quality. Automating repetitive tasks or using AI to handle certain types of calls can help alleviate the burden on operators.

- Providing additional training and support to operators who handle a high volume of calls can help them manage calls efficiently, even during peak demand periods.
