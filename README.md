# Crime Analysis Project

## Authors:
- Derek Schiltz
- Khoa Cao
- Taran Patel
- Tianyi Xu

## Date:
April 4, 2023

## Project Overview:
This project analyzes arson crime data collected by the Los Angeles Police Department (LAPD). The primary goal of this analysis is to investigate whether arson crimes with weapon involvement are more likely to occur during late evening hours compared to early morning hours. Using hypothesis testing and statistical inference, the project aims to compare weapon presence proportions during these two time periods.

## Data:
The dataset used for this analysis is publicly available from the LAPD and can be accessed [here](https://catalog.data.gov/dataset/crime-data-from-2020-to-present). The dataset contains records of crime incidents in Los Angeles from 2020 to the present. The key variables used in this analysis include:
- `Month Occurred`: Month of the crime.
- `Time Occurred`: Time of day the crime occurred, categorized into sections (e.g., Early Morning, Late Evening).
- `Crime Description`: Type of crime (focused on "Arson" for this study).
- `Weapon Presence`: Whether a weapon was involved in the crime.

## Key Questions:
The primary question guiding this analysis is:
- For all "arson" crimes, is it significantly more likely for a weapon to be involved in the late evening compared to the early morning?

## Methodology:
1. **Data Cleaning and Transformation**: The dataset was cleaned and filtered to include only relevant variables. The `Time Occurred` variable was categorized into six time periods: Overnight, Early Morning, Morning, Afternoon, Early Evening, and Late Evening. The presence of a weapon was categorized as either "Weapon Present" or "No Weapon."

2. **Hypothesis Testing**: A one-sided z-test was conducted to compare the proportions of arson crimes with weapon presence during the late evening and early morning hours.

3. **Graphs and Visualization**: The project includes visualizations showing:
   - The proportion of arson crimes by time of day.
   - The proportion of weapon presence during arson crimes for different times of day.

4. **Inference Procedure**:
   - The null hypothesis is that there is no difference in the proportion of arson crimes involving weapons between the late evening and early morning.
   - The alternative hypothesis is that the proportion of arson crimes involving weapons is higher during the late evening than in the early morning.

## Results:
The results showed that the weapon presence proportion for late evening arson crimes was 0.312, while for early morning arson crimes, it was 0.259. However, the calculated p-value was 0.071, which is greater than the significance threshold of 0.05. Therefore, the null hypothesis could not be rejected, meaning there is insufficient evidence to suggest a significant difference between the two time periods.

## Discussion:
While this analysis did not provide statistically significant evidence that arson crimes with weapon involvement are more likely during the late evening compared to the early morning, the results are close to the threshold of significance. Increasing the sample size or adjusting the threshold could lead to different conclusions. Additionally, limitations such as non-random data collection and potential underreporting of crimes should be considered when interpreting the results.

Future analyses could explore other factors, such as the day of the week or geographical location, and apply different statistical models or simulations to further validate the findings.

## Dependencies:
This project requires the following libraries:
- `tidyverse`
- `lubridate`

Additional helper scripts:
- `viridis.R`
- `ggprob.R`

## Conclusion:
This project provides an analysis of the relationship between time of day and weapon presence in arson crimes in Los Angeles. While no significant difference was found in this study, further analysis could yield different insights.
