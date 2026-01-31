# Vehicle-thefts-data-analysis
An analysis of New Zealand vehicle thefts for the 6 month period ending April 6th 2021. 
Data was made up of three tables: 
* "stolen vehicles" fact data containing the details of each theft
* "make details" dimension data containing manufacturer and luxury/standard flag
* "locations" dimension data with region and population data.

Data was downloaded from Maven Analytics. 
## Data preparation and cleansing
### Using Snowflake SQL
* Fixed dates whose year was 0022 and 0021. [Please see here for SQL used.](https://github.com/diggooddodg/Vehicle-thefts-data-analysis/blob/main/detail%20/Snowflake%20SQL%20-%20cleaning.md)
### Using Excel
* Created a calendar lookup table for use in Power BI
* The following cleaning steps were performed on the stolen vehicles table using MS Excel:
  * Removed blank rows
  * Null vehicle descriptions changed to "Unknown"
  * Fixed trailer descriptions so that they were consistent ("home built" now part of "homemade")

## Power BI
Data was imported to Power BI. [Screenshots may be seen here](https://github.com/diggooddodg/Vehicle-thefts-data-analysis/blob/main/detail%20/Power%20BI%20screenshots.md)

## Snowflake SQL
Data was uploaded to Snowflake and queries performed to determine various metrics including the following. [Please see here for SQL used.](https://github.com/diggooddodg/Vehicle-thefts-data-analysis/blob/main/detail%20/%20Snowflake%20SQL%20-%20Vehicle%20thefts.md)
* Number of thefts in total
* Most stolen type of car
* Most stolen make / model
* Regions with the highest thefts and highest thefts per capita
* Thefts by day of week
* Average age of vehicles when stolen

## Summary PowerPoint
Summary of findings may be seen here:
