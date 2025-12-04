# hackapaws_capstone_project
The project is comparing the mortality rates of US citizens with the number of medicinal sales from 2015-2025. We have used 2 different datasets one of the US death rate and the other of the medicinal sales over the years. We have used different data analytical operations like data cleansing, data visualisation and recording the final results and conclusion.


## Data Sources

-   **U.S. Death Records**: `/content/us_death_records_by kaushal patidar.csv`
    *   *Description*: Contains information about death records, including cause of death, demographics, and location.
    *   *Link*: https://drive.google.com/file/d/1L8GWB3JH7G4rvqR1lbRD7wLIazEarJ7y/view?usp=drive_link

-   **Unified Health Medicine Sales**: `/content/unified_health_2020_2025_realnames.csv`
    *   *Description*: Contains data on medicine sales, recovery rates, government spending, and hospital information.
    *   *Link*: https://drive.google.com/file/d/1jTxnUs1sTjcaXyzbDT1A6yQ8ubY9WobK/view?usp=drive_link
 
## Data cleaning

-  **Renaming** :
   * Trying to maintain the consistency of the data, renamed the Cause_of_death column to Disease_name so, that the aggregation of two datasets would be easy.
-  **Data standardisation** : 
   * To maintain the data standardisation, we took some disease name like accident_injuries or chronic diseases as others and the influenza & neumonia as influenza only.

## Data merging

-  **Important Columns** :
   * The important columns for two datasets to merge is Year and Disease_name, we tried to analyse how the average recovery rate affected per disease pre - 2021 and post - 2021.

## Analysis

- **policy change analysis** :
  * How the average recovery rate for the kidney disease and some other disease got really high then the other diseases.
- **correlation** :
  * The correlation for kidney disease and some disease has positive correlation while, others has the negative correlation.
  * We trying to find the pearson correlation value for avg_recovery_rate vs the total_units_sold was in the positive direction.
  * the pearson correlation for total_units_sold vs the government_spending_millions was in the negative direction.
  * We also performed the hypothesis testing, in which we got no significance difference after putting the alpha value of 0.05, as every disease recovery rate pre-2021 and post-2021 was higher then the expected threshold

## Visualisations 

* we tried to put every findings in the bar graph and also tried to analyse it in different aspeccts, as comparing it with the hospital type or insurance type or number of comorbidities or the state wise that, does it actually makes any difference in the recovery rate of the US citizens.
* we have used heatmap to get an idea how some variables affecting the other variables.

## Conclusion and summary 

* we concluded that the recovery rate for the US citizen doesn't actually affected by the number of medicinal sales or the government spending, it actually affected on the basis of the disease and not acutally on anything
* In our dataset the data rows and columns are really less so, we can't actually say that correlation we did does it actually casuing causation or not because, the pearson correlation was just the introductory step to show the relationship between two variables.
* As in the data cleaning part, we renamed the column to another column name for maintaining the consistency and as, we had less number of data to work with we didn't had to look for the null values but, what if it was a large dataset then, it may cause some issues with the current scenario.
