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

