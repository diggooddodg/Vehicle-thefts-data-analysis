# Data preparation and cleanse
Data was in csv format and made up of three tables: 
* "stolen vehicles" fact data containing the details of each theft
* "make details" dimension data containing manufacturer and luxury/standard flag
* "locations" dimension data with region and population data.
Data was downloaded from Maven Analytics.

## Data preparation and cleanse using Excel
* Created a calendar lookup table for use in Power BI
* The following cleaning steps were performed on the stolen vehicles table using MS Excel:
  * Removed blank rows
  * Null vehicle descriptions changed to "Unknown"
  * Fixed trailer descriptions so that they were consistent ("home built" now part of "homemade")

## Data cleaning performed in Snowflake SQL
When calculating vehicle age in Snowflake the values were negative, this led to the following investigation and fix. (As can be seen below during import to Snowflake, some years were automatically changed to 0022 and 0021.)
### Check theft counts by year
<img width="760" height="342" alt="image" src="https://github.com/user-attachments/assets/9a108aa4-dc67-43f4-bd01-a3de27721e97" />

### Double check by viewing original year values
<img width="188" height="35" alt="image" src="https://github.com/user-attachments/assets/976e0dce-dcbb-41d5-add3-78846c127283" />
<br>
<img width="737" height="267" alt="image" src="https://github.com/user-attachments/assets/baee5dcf-c035-4c4c-bba0-72ad6cfabda0" />




### Apply fix
<img width="753" height="296" alt="image" src="https://github.com/user-attachments/assets/3aaf106d-ec93-4ddf-87f1-872943e22086" />


### Check again
<img width="757" height="266" alt="image" src="https://github.com/user-attachments/assets/66ab7d8f-6361-47b1-8586-afc0d0443ff3" />


