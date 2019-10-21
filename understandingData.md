# Necessary Data for a Basic Predictor
* Team ID's and Team Names
* Tournament seeds since 1984-85 season
* Final scores of all regular season, conference tournament, and NCAA® tournament games since 1984-85 season
* Season-level details including dates and region names (year is when march madness is)

# Data Section 1 - The Basics
* Teams.csv
  * TeamID: 4 digit id
  * TeamName: team name (16 char limit)
  * FirstD1Season: first season the team was in division 1 (post 1985)
  * LastD1Season: last season the team was in division 1 (current teams in division will will have LastD1Season=2019)
* Seasons.csv
 * Season: year which tournament was played (current is 2019)
 * DayZero: date corresponding to daynum=0 (first day of season)
 * RegionW,RegionX,RegionY,RegionZ: 
* NCAATourneySeeds.csv
  * Season
  * Seed
  * TeamID
* RegularSeasonCompactResults.csv
  * Season
  * DayNum
  * WTeamID
  * WScore
  * LTeamID
  * LScore
  * WLoc
  * NumOT
* NCAATourneyCompactResults.csv
* SampleSubmissionStage1.csv
  * ID
  * Pred


# Data Section 2 - Team Box Scores
* RegularSeasonDetailedResults.csv
* NCAATourneyDetailedResults.csv

# Data Section 3 - Geography
* Cities.csv
 * CityID: 4 digit id
 * City: name of city
 * State: abbreviation of state
* GameCities.csv
 * Season,DayNum,WTeamID,LTeamID: uniquely identify each game
 * CRType: regular (RegularSeasonCompactResults.csv), NCAA (NCAATourneyCompactResults.csv), Secondary (SecondaryTourneyCompactResults file)
 * CityID: id of city where game was played (correspond to Cities.csv)


# Data Section 4 - Public Rankings
* MasseyOrdinals.zip containing MasseyOrdinals.csv
  * Season: year associated with Seasons.csv
  * RankingDayNum: first day to use rankings for predicted games (ex. if RankingDayNum=110, then rankings based on days 0-109)
  * SystemName: 3 letter abbreviation of each ranking system
  * TeamID: id of team being ranked (Teams.csv)
  * OrdinalRank: overall ranking of team in underlying system (out of 353)

# Data Section 5 - Play by Play
* PlayByPlay_201X.zip containing Events_201X.csv and Players_201X.csv
* Events_201X.csv
  * EventID: id for each logged event
  * Season,DayNum,WTeamID,LTeamID: uniquely identify each game (mix of regular season,NCAA tourney,and Secondary tourney)
  * WPoints,LPoints: points added in perspective of winning team (1,2 or 3)
  * ElapsedSeconds: seconds elapsed from the start of the game until event occured (0-1200 first half,12-2400 second half,above 2400 overtime)
  * EventTeamID: id of the team that the event is logged for (either WTeamID or LTeamID)
  * EventPlayerID: id of the player that the event is logged for (correspond with Players_201X.csv)
  * EventType: type of event that was logged (assist,block,steal,turnover,timeout/timeout_tv,foul_pers/foul_tech,reb_off/reb_def/reb_dead,sub_in/sub_out,made1free/miss1_free,made2_dunk/miss2dunk,made2_tip/miss2_tip,made2_lay/miss2_lay,made2_jump,miss2_jump,made3_jump/miss3_jump)
* Players_201X.csv
  * PlayerID: id for players (different within each year)
  * Season: year of the associated entry
  * TeamID: players team id
  * PlayerName: player's name (LAST_FIRST)

# Data Section 6 - Supplements
* TeamCoaches.csv
* Conferences.csv
* TeamConferences.csv
* ConferenceTourneyGames.csv
* SecondaryTourneyTeams.csv
* SecondaryTourneyCompactResults.csv
* TeamSpellings.csv
* NCAATourneySlots
* NCAATourneySeedRoundSlots.csv
