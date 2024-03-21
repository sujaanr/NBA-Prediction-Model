

# Predicting Sports Using a Logistic Regression Model in Python

# Model
In my journey to predict NBA game outcomes more accurately, I've developed a logistic regression model that meticulously analyzes eight critical factors, each normalized per 100 possessions. This normalization is crucial as it accounts for the pace of the game, ensuring that our predictions are not just accurate but also universally applicable, regardless of the game's tempo. The factors my model considers include:

- Home Team Advantage: Recognizing the statistical boost teams often receive when playing on their home court.

- Win Percentage: A direct indicator of a team's performance and momentum.

- Rebounds: Essential for understanding a team's control over the ball and the game.

- Turnovers: Indicative of a team's discipline and handling under pressure.

- Plus/Minus: A snapshot of team performance when specific players are on the court.

- Offensive Rating: Measures a team's efficiency at scoring points.

- Defensive Rating: Gauges a team's effectiveness in preventing the opponent from scoring.

- True Shooting Percentage: A more accurate measure of a player's shooting efficiency, considering field goals, 3-point field goals, and free throws.

 
# Usage

### **Installation**

```bash
pip3 install -r requirements.txt
```

### **Daily Predictions**
1. Navigate to and open nbaPredict.py.
2. Adjust the call to makeInterpretPrediction with your desired game date, season, and the season's start date.
3. Execute the script via terminal or your preferred IDE.
4. Allow approximately 1-3 minutes for the model to scrape the necessary stats and predict game outcomes.
5. Predictions will be presented as the percent chance of the home team winning against the away team.

### **Past Predictions**
1. Open makePastPredictions.py
2. Edit the call to makePastPredictions with desired start date, end date, season, start date of the season, and output
filenames. NOTE: The start date should be at least three days after the season begins and the end date is non-inclusive.
3. Run the program either through the terminal or an IDE
4. Two CSV files will be saved in the Data folder. One holds the gameData and the other holds the predictions for the games. The time to execute will vary greatly from a couple minutes to a several hours depending on the range between the start and end date.
