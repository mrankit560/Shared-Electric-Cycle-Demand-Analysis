# Yulu: Hypothesis Testing

## About Yulu
Yulu is India’s leading micro-mobility service provider, offering unique vehicles for daily commutes. Launched to tackle traffic congestion in India, Yulu provides a safe commute solution through a user-friendly mobile app, enabling shared, solo, and sustainable commuting. Yulu zones are strategically located at key areas (metro stations, bus stands, office spaces, residential areas, etc.) to ensure smooth, affordable, and convenient commutes.
 
Recently, Yulu has experienced significant dips in revenue. They have contracted a consulting company to identify the factors affecting the demand for shared electric cycles in the Indian market.
 
## Objective
The main objectives of this project are to answer the following questions:
- Which variables are significant in predicting the demand for shared electric cycles in the Indian market?
- How well do those variables describe the demand for electric cycles?

## Dataset
- **Dataset Link**: [yulu_data.csv](https://drive.google.com/file/d/1aui7GEjCuBg1a2Nl3jHnIOkXZJL_3ajV/view)
- **Column Profiling**:
  - `datetime`: datetime
  - `season`: season (1: spring, 2: summer, 3: fall, 4: winter)
  - `holiday`: whether the day is a holiday or not (extracted from [DCHR Holiday Schedule](http://dchr.dc.gov/page/holiday-schedule))
  - `workingday`: if the day is neither a weekend nor a holiday is 1, otherwise is 0.
  - `weather`:
    - 1: Clear, Few clouds, Partly cloudy
    - 2: Mist + Cloudy, Mist + Broken clouds, Mist + Few clouds, Mist
    - 3: Light Snow, Light Rain + Thunderstorm + Scattered clouds, Light Rain + Scattered clouds
    - 4: Heavy Rain + Ice Pallets + Thunderstorm + Mist, Snow + Fog
  - `temp`: temperature in Celsius
  - `atemp`: feeling temperature in Celsius
  - `humidity`: humidity
  - `windspeed`: wind speed
  - `casual`: count of casual users
  - `registered`: count of registered users
  - `count`: total count of rental bikes, including both casual and registered users

## Concepts Used
- Bi-Variate Analysis
- 2-Sample T-Test: Testing for differences across populations
- ANOVA
- Chi-Square

## How to Begin
1. Import the dataset and perform exploratory data analysis (EDA) to check the structure and characteristics of the dataset.
2. Establish relationships between the dependent variable (`count`) and independent variables (e.g., `workingday`, `weather`, `season`).
3. Select appropriate tests to check:
   - Whether `workingday` affects the number of electric cycles rented.
   - If the number of cycles rented is similar or different in different seasons.
   - If the number of cycles rented varies with different weather conditions.
   - The dependency of `weather` on `season`.
4. Set up the Null Hypothesis (H0) and the Alternate Hypothesis (H1).
5. Check assumptions of the tests (Normality, Equal Variance) using histograms, Q-Q plots, or statistical methods like Levene’s test or Shapiro-Wilk test.
6. Set a significance level (alpha).
7. Calculate test statistics.
8. Make decisions to accept or reject the null hypothesis.
9. Draw inferences from the analysis.

## Results Overview
- Analyzed 10,886 Yulu bike rental data points from January 2011 to December 2012.

### Key Metrics:
- Assessed bike rentals based on weather, seasonality, and time of day.
- Seasonal trends indicate higher demand during summer and fall, with winter showing the highest rentals.
- Peak rentals occurred between 12 PM and 6 PM, with similar demand on weekdays and weekends.
- Clear weather resulted in 7,192 rentals, while heavy rain led to only 1 rental.
- Rentals peaked between 20.5°C and 26.24°C, with higher humidity reducing demand.
- No significant difference in rentals between working and non-working days.
- Recommendations include optimizing bike availability during peak periods, weather-based pricing, and seasonal marketing campaigns.

## Recommendations
1. Optimize bike distribution in peak months (June, July, August).
2. Implement seasonal marketing strategies to leverage demand trends.
3. Enhance user engagement through targeted promotions during off-peak months.
4. Consider dynamic pricing strategies based on weather conditions.
5. Explore additional revenue streams through partnerships or premium services.
6. Invest in technology and infrastructure to improve user experience.
7. Adjust bike deployment strategies based on demand patterns.
8. Adapt promotions based on weather conditions.
9. Advertise differently in each season.
10. Plan bike availability considering both season and weather.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgements
- Yulu for providing the dataset and context for analysis.
