# Shared Electric Cycle Demand Analysis

## Overview
This project focuses on analyzing the factors affecting the demand for shared electric cycles for a leading shared mobility provider in the urban transportation sector. The analysis employs hypothesis testing methods to understand how various external factors, such as weather conditions and weekdays, influence the usage patterns of shared electric cycles.

## Problem Statement
The primary objective is to identify significant factors that drive the demand for shared electric cycles, thereby providing actionable insights for optimizing fleet distribution, pricing strategies, and marketing campaigns.

## Dataset Overview
The dataset consists of records related to electric cycle rentals, including the following attributes:
- **Rental ID**: Unique identifier for each rental transaction.
- **Rental Date**: Date and time of the rental.
- **Weather Condition**: Weather status during the rental period (e.g., sunny, rainy).
- **Working Day**: Indicator of whether the day is a working day or weekend.
- **Season**: The season during which the rental occurred (e.g., summer, winter).
- **Rental Duration**: Duration for which the cycle was rented (in hours).

## Analysis Objectives
This analysis aims to address key questions regarding the demand for shared electric cycles:
- How do weather conditions impact rental rates?
- Do rentals vary significantly between weekdays and weekends?
- What seasonal trends can be identified in rental data?
- Are there significant differences in rental durations based on external factors?

## Methodology
1. **Exploratory Data Analysis (EDA)**: Initial data exploration to understand trends and patterns in the dataset.
2. **Hypothesis Formulation**: Formulating null and alternative hypotheses for various factors impacting rental demand.
3. **Statistical Testing**: Conducting 2-sample T-tests and ANOVA tests to assess the significance of factors affecting rental rates.
4. **Chi-Square Tests**: Analyzing categorical variables to evaluate their relationship with rental behaviors.
5. **Visualization**: Creating visual representations of the data to highlight trends and insights effectively.

## Insights
- The analysis revealed that demand for shared electric cycles significantly increases during sunny weather conditions, with peak rentals occurring on weekends.
- Rental durations are longer during summer months compared to winter, indicating seasonal preferences among users.
- A notable increase in rentals was observed on public holidays, suggesting that external factors can heavily influence demand.

## Recommendations
Based on the findings, the following recommendations are proposed:
1. **Dynamic Pricing**: Implement a dynamic pricing strategy that adjusts rental rates based on weather forecasts to maximize revenue during peak demand periods.
2. **Optimized Fleet Distribution**: Utilize insights on peak rental times to optimize fleet distribution, ensuring that cycles are available in high-demand areas.
3. **Targeted Marketing Campaigns**: Develop marketing campaigns that promote cycle rentals during favorable weather conditions and on weekends to boost user engagement.

## Technologies Used
- **Python**: For data analysis and hypothesis testing.
- **Libraries**: pandas, NumPy, SciPy, Matplotlib, Seaborn.

## How to Use This Repository
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/repository-name.git
   ```
2. Open the Jupyter notebook (`bike_sharing_by_ankit.ipynb`) to explore the detailed analysis and insights derived from the dataset.
3. Review the dataset file (`bike_sharing.csv`) for a comprehensive view of the rental data used in the analysis.

## License
This project is licensed under the MIT License - see the LICENSE file for details.
