# Vehicle-thefts-data-analysis
An analysis of NZ vehicle thefts for the 6 month period ending April 6th 2021. 
Data was made up of three tables: 
* "stolen vehicles" fact data containing the details of each theft
* "make details" dimension data containing manufacturer and luxury/standard flag
* "locations" dimension data with region and population data.

Data was downloaded from Maven Analytics. 
## Data preparation and cleansing in Excel
* Created a calendar lookup table for use in Power BI
* The following cleaning steps were performed on the stolen vehicles table using MS Excel:
  * Removed rows with null primary key, vehicle type and make id
  * Null vehicle descriptions changed to "Unknown"
  * Fixed trailer descriptions so that they were consistent ("home built" now part of "homemade")
## Power BI
### Overview
<img width="1410" height="794" alt="Vehicle thefts1" src="https://github.com/user-attachments/assets/27df251a-e912-48b7-822e-a021963743e7" />

### Regional
<img width="1399" height="800" alt="Vehicle thefts2" src="https://github.com/user-attachments/assets/b9b9594c-794d-44fc-846d-bb6b4a95e331" />

### Correlation with regional population
<img width="1414" height="796" alt="Vehicle thefts3" src="https://github.com/user-attachments/assets/22a64c9a-6ee3-4ff0-ad02-d4c692ea47a6" />

## Snowflake SQL
Data was uploaded to Snowflake and several queries performed

## Summary PowerPoint
Summary of findings may be seen here:
