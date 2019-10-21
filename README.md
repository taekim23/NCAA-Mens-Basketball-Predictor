# NCAA-Mens-Basketball-Predictor
Explore Kaggle's 2019 NCAA Mens Basketball dataset and create a predictor to predict future tournament winners

Getting Dataset:
1. pip install kaggle
2. Sign up for Kaggle account (https://www.kaggle.com) 
3. Verify phone number for account
4. Go to My Account
5. Click Create New API Token (will download a kaggle.json file)
6. Place the kaggle.json file in the .kaggle folder created by installing kaggle (C:/users/username/.kaggle)
7. Accept the rules of the competition (https://www.kaggle.com/c/mens-machine-learning-competition-2019/data → click download all)
8. kaggle competitions download -c mens-machine-learning-competition-2019 (cmd function)
	
Preprocessing Steps: 

Data to Look at: 
* Most tourney wins since 1985
* Conference with most wins
* Seeds with most titles
* Seeding Performance in the tourney (each round)
* Higher seeds winning percentage through the season
* Pomeroy/Sagarin Ranking
* Relationship between winning margin and ranking difference
* Averages (points per game, possessions per game, three pointers made and attempted, average free throws made and attempted, average assists, average defensive records)
* Advanced Stats (Possessions, Offensive Rating, Defensive Rating, Strength of Schedule, Performance Impact Estimator (PIE), Team Impact Estimator (TIE), Assist ratio, Turnover ratio, True Shooting %, Effect FG%, Free Throw Rate, Offensive Rebound %, Defensive Rebound %, Total Rebound %)
* Tournament vs Regular Season Stats (Points,Field Goals,Rebounds,)
* Statistics and wins (Field Goal Attempts, Field Goals made, Threes made, Free throws made, Free throws attempted offensive rebounds, defensive rebounds, blocks, steals, possessions, turnovers, personal fouls)

