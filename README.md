# Covid19 Data - Switzerland
Demo Project to import, analyze and visualize Covid Data from Switzerland. Developed with Python, JupyterNotebook and VSCode.

## Data Science
Import of daily Covid data from OpenZH (Source described below). Data is preprocessed and cleaned. Output is stored in a CSV File (Data/CovidData) and Archived (Data/Archive).
- [Data preprocessing](https://github.com/cschweizer/datascience-covid19-data-switzerland/blob/master/01%20Data%20Import/ImportData.ipynb)
- [Descriptive Analytics](https://github.com/cschweizer/datascience-covid19-data-switzerland/blob/master/02%20Data%20Analytics/DescribtiveAnalytics.ipynb)
- [Visualization](https://github.com/cschweizer/datascience-covid19-data-switzerland/blob/master/02%20Data%20Analytics/Visualizations.ipynb)

## Project
Projet Setup and Packages used for this Project. 
Ideas for further Implementations.

### Setup
- pip3 install requests
- pip3 install pandas
- pip3 install seaborn
- pip3 install plotly

### Ideas
- Vaccination
- Positivitätsrate
- externe Sources (Wetter, Stringency Index)
- Descriptive: Total Infizierte / Geimpfte / % ..
- Visualization mit GeoPandas

## Data
Data Source, Processing and Documentation of the Output Data.
### Sources
OpenZH (Specialist Unit for Open Government Data Canton of Zurich): https://github.com/openZH/covid_19

### Processing
- Aggregates all Cantons in one Dataset
- Add Daily Numbers (Tested, Confirmed, Released, Deceased)
- Add seven day means for Confirmed and Deceased Cases

### Structure
#### 'date'
Date when the numbers where reported

#### 'canton'
Canton in which the numbers where reported

#### 'daily_tested'
Amount of tests per day

#### 'ncumul_tested'
Ammount of tests total

#### 'daily_conf'
Amount of positive tests per day

#### 'ncumul_conf'
Amount of positive tests total

#### 'seven_day_conf'
Seven Day mean of positive tests per days

#### 'testRelation'
% positive tests to total tests

#### 'new_hosp'
Amount of new hospitalisations per day

#### 'current_icu'
Amount of ICU patients

#### 'current_vent'
Amount of patients which needs vent

#### 'ncumul_released'
Amount of released patients total

#### 'daily_released'
Amount of released patients per day

#### 'daily_deceased'
Amount of deceased patients per day

#### 'ncumul_deceased'
Amount of deceased patients total

#### 'seven_day_dec'
Seven day mean of deceased patients

#### 'current_isolated'
Total amount of persons which are currently isolated

#### 'current_quarantined_total'
Total amount of persons which are currently quarantined