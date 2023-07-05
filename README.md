# Capstone

# Capstone Tableau Link
[Yaw Agyekum's Capstone](https://public.tableau.com/app/profile/yaw.agyekum/viz/SavvyCapstone_16884332029590/PredictGoals?publish=yes)

<br>
<br>

## Dataset Link
[2022-2023 Top 5 Football Leagues Player Stats](https://www.kaggle.com/datasets/joyshil0599/2022-2023-top-5-football-leagues-player-stats)
<br>
<br>



### Using Predictive Analysis, I created column PredictGoals and the formula ((Goal + Expected Goal + NonPenaltyExpectedGoal) / Minutes Played) * 90 to predict who scores in the next game in all 5 top European leagues namely:
<br>
<br>

### Bundesliga: a professional association football league in Germany. At the top of the German football league system, the Bundesliga is Germany's primary football competition. The Bundesliga comprises 18 teams and operates on a system of promotion and relegation...


### La Liga:  a private sports association composed of the 20 clubs and SADs (public limited sports companies) in LaLiga Santander and the 22 in LaLiga SmartBank, responsible for the organisation of these national professional football competitions.


### Ligue 1: officially known as Ligue 1 Uber Eats for sponsorship reasons, is a French professional league for men's association football clubs. At the top of the French football league system, it is the country's primary football competition.


### Premier League: legal name: The Football Association Premier League Limited, is the highest level of the men's English football league system. Contested by 20 clubs, it operates on a system of promotion and relegation with the English Football League (EFL).


### Serie A: is regarded as one of the best football leagues in the world and it is often depicted as the most tactical and defensively sound national league.
### In this dataset, we will be using performance metrics ranging from number of matches played, minutes played, goals, assists, passes, etc. 
<br>
<br>


## Dataset Cleaning Techniques
### In Python, I replace the nulls with empty space and rename some of the columns: "compition", "Born year", "MIn", "Progressive Carries", "Progressive Passes", "Progressive Passes Receive".
### Deleted some columns including "Goal + Penalty kick", "Penalty Kick", "Penalty Kick Attempted", "Yellow Card", "Red Card", "Non-penalty Expected Goal", "Expected Assisted Goal", "Non-penalty Expected Goal + Expected Assisted Goal".
### Saved to CleanedPlayerStatsPython.csv
<br>
<br>


### Imported CleanedPlayerStatsPython.csv to SQLite, saved it as CleanedPlayerStatsSQL.csv and did the following:
### Renamed the position and adjusted their ages from decimal to int.
### Also, set NULL to zero and cast goals from a decimal to a integer.
### Exported CleanedPlayerStatsSQL.csv as an Excel file as CleanedPlayerStatsExcel.xlsx
<br>
<br>


### In Excel, I added a column PredictGoals with the formula (Goal + Expected Goal + NonPenaltyExpectedGoal) / Minutes Played) * 90
<br>
<br>

### Imported CleanedPlayerStatsExcel.xlsx into Tableau for the data visualization