# OlympicGamesAnalysis-usingSQL-PowerBI
Exploring and analysing key insights from Olympic games data  & building an interactive dashboard using SQL and PowerBi

#### Objective
Ensuring that the right data has been selected,transformed and used in the data visualization which is meant to be passed on to the business users. Here We have to visulaize the data which will help readers to understand how countries have performed historically in the summer Olympic games with a possibility to select our own country and also we should find if there is anything interesting about the competitors.


#### About the dataset
The data we are exploring is about Olympic games from 1896-2016 which we downloaded from google.
This data was first put into a SQL database and afterwards transformed using the SQL query which can be found in the .sql file attached with this project


#### Calculations
The following calculations were created in the Power BI reports using DAX (Data Analysis Expressions)

No of Competitors = DISTINCTCOUNT( ‘Olympic Data'[ID] )

No of Medals = COUNTROWS( ‘Olympic Data’ )

No of Medals (Registered) = CALCULATE( [No of Medals], FILTER( ‘Olympic Data’, ‘Olympic Data'[Medal] = “Bronze” || ‘Olympic Data’ [Medal] = “Gold” || ‘Olympic Data'[Medal] = “Silver” ))


#### About the Dashboard
The finished dashboard consist of visualizations and filters that gives an easy option for the end users to navigate the summer games through history. Some possibilities are to filter by period using year, nation code to focus on one country or look into either a competitor or specific sports over time.
