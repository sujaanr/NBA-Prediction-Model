# predicting sports using a logistic regression model in python

## model
in my journey to predict nba game outcomes more accurately, i've developed a logistic regression model that meticulously analyzes eight critical factors, each normalized per 100 possessions. this normalization is crucial as it accounts for the pace of the game, ensuring that our predictions are not just accurate but also universally applicable, regardless of the game's tempo. the factors my model considers include:

- home team advantage: recognizing the statistical boost teams often receive when playing on their home court.
- win percentage: a direct indicator of a team's performance and momentum.
- rebounds: essential for understanding a team's control over the ball and the game.
- turnovers: indicative of a team's discipline and handling under pressure.
- plus/minus: a snapshot of team performance when specific players are on the court.
- offensive rating: measures a team's efficiency at scoring points.
- defensive rating: gauges a team's effectiveness in preventing the opponent from scoring.
- true shooting percentage: a more accurate measure of a player's shooting efficiency, considering field goals, 3-point field goals, and free throws.

## usage

### installation

```bash
pip3 install -r requirements.txt
```
### **daily predictions**
1. navigate to and open nbapredict.py.
2. adjust the call to makeinterpretprediction with your desired game date, season, and the season's start date.
3. execute the script via terminal or your preferred ide.
4. allow approximately 1-3 minutes for the model to scrape the necessary stats and predict game outcomes.
5. predictions will be presented as the percent chance of the home team winning against the away team.

### **past predictions**
1. open makepastpredictions.py
2. edit the call to makepastpredictions with desired start date, end date, season, start date of the season, and output filenames. note: the start date should be at least three days after the season begins and the end date is non-inclusive.
3. run the program either through the terminal or an ide
4. two csv files will be saved in the data folder. one holds the gamedata and the other holds the predictions for the games. the time to execute will vary greatly from a couple minutes to a several hours depending on the range between the start and end date.

