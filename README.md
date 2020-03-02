# Final-Project

## Horse Racing: An analysis to predict 2020 outcomes

Use Scikit-learn, Python Pandas, Google Cloud SQL to analyze existing horse racing data to create a classification model that will predict future outcomes. 

### Analysis 
Research shows "All independent variables (age, breed, sex, gait, track surface and total number of starts) had a significant impact on total earnings.”(1)

<a href="https://console.cloud.google.com/bigquery?folder=true&organizationId=true&orgonly=true&project=final-project-269915&supportedpurview=project&j=bq:US:bquxjob_51b444c6_1709be1f532&page=queryresults">Big Query</a>
- Datasize: 27k
- horse weight, jockey, finish place
- Finish place -> boolean winner column: place = 1 (true), place = >=2 (false)
- <a href="https://datastudio.google.com/u/0/explorer/7454d1e9-8bd8-4e29-a638-e4e725399b48">Data Studio Viz</a>
-- Big Query, SQL 

<a href="http://localhost:8888/notebooks/FinalProject_OverallPredicts.ipynb">Overall</a>
- Datasize: 44k rows 
- Random Forest: dam id, sire id, trainer id, rider id, prize money, handicap weight, age, sex id
- Logistic Regression

<a href="http://localhost:8888/notebooks/FinalProject_KentuckyDerby.ipynb#.ipynb">Kentucky Derby</a>
- Datasize: 235 rows, KDerby Data 2008 - 2019 
- Random Forest: Starters, Dosage Index (calculated based on an analysis of the horse's pedigree), Finish Position (Place_Bins)
- Predict_Proba
- Pickeled Model 


#### Data Sources
- Horse Racing Datasets: http://horseracingdatasets.com/kentucky-derby/
- Data.World: https://data.world/sya/horses-for-courses/workspace/query?filename=runners.csv%2Frunners.csv&newQueryType=SQL&selectedTable=runners&tempId=1583168958109

#### Other Sources
1. Relationships between race earnings and horse age, sex, gait, track surface and number of race starts for Thoroughbred and Standardbred racehorses in North America: https://beva.onlinelibrary.wiley.com/doi/abs/10.1111/j.2042-3306.2010.00032.x
