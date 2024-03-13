

Predicts NBA Games Using a Logistic Regression Model in Python

# Model
Our logistic regression model incorporates eight crucial factors, each normalized to per 100 possessions to neutralize pace impact, ensuring our predictions are both accurate and reliable. The factors include:

Home Team Advantage
Win Percentage
Rebounds
Turnovers
Plus/Minus
Offensive Rating
Defensive Rating
True Shooting Percentage

# Usage

### **Installation**

```bash
pip3 install -r requirements.txt
```

### **Daily Predictions**
1. Open nbaPredict.py
2. Edit the call to makeInterpretPrediction with desired date of games, season, and the start date of the season
3. Run the program either through the terminal or an IDE
4. Wait ~1-3 minutes for model to finish scraping stats and predicting outcomes
5. Outcomes are outputted as the percent chance that the home team will defeat the away team

### **Past Predictions**
1. Open makePastPredictions.py
2. Edit the call to makePastPredictions with desired start date, end date, season, start date of the season, and output
filenames. NOTE: The start date should be at least three days after the season begins and the end date is non-inclusive.
3. Run the program either through the terminal or an IDE
4. Two CSV files will be saved in the Data folder. One holds the gameData and the other holds the predictions for the games. The time to execute will vary greatly from a couple minutes to a several hours depending on the range between the start and end date.
