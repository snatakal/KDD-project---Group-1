# League of Legends Game analysis - Group-1

## Team Members:

Tarun Ravada
Vishwath Kamalanathan
Swetha Natakala Ramakumar
Adithi Macherla

## Project Description:

### Introduction:

League of Legends, commonly referred to as League, is a highly popular Multiplayer online battle arena game. The game annually hosts the League World Championship, which has one of the largest prize pools in e-sports. As such there are high stakes involved for the participating teams, sponsors of teams, and the viewers. Teams spend a lot of time analyzing different team compositions, matchups, and strategies to maximize their chances of winning each match.

Every match of League has many factors that affect the outcome of the match. Some examples of these factors are: the playable character (champion) being played, the number of enemy kills a player had, the amount of gold a player earned, etc. Data analytics is used to understand the relationships between these factors so that teams can prioritize and adapt to the different changes that each match brings about.

### Data:

The initial data source for this project is a large data set consisting of in-game statistics of players playing League at the Master rank level. The dataset was obtained from [Kaggle](https://www.kaggle.com/jasperan/league-of-legends-1v1-matchups-results). Additional game data will be obtained from League servers using the Riot Games [API](https://developer.riotgames.com/docs/lol). 

A description of the dataset is provided in the Data Understanding section below.

### Installation:

Anaconda 4.10.1 Distribution
Python 3.9.5
Jupyter Notebook 

## CRISP-DM Process:

The Cross-Industry Standard Process for Data Mining (CRISP-DM) is a tried-and-true mechanism for directing your data mining efforts. As a methodology, it includes descriptions of common project phases, associated tasks, and explanations of the links between these tasks.

- Business Understanding
- Data Understanding
- Data Preparation

### Business Understanding:

This phase comprises of outlining a detailed description of the problem as well as procedures for assessing whether or not the goal has been met.

PROBLEM → MODEL → SOLUTION

For this project, we are trying to understand:

- How in-game factors such as gold earned, vision score, and creep score affect the outcome of the game. 
- How champion matchup effects the in-game factors of a player.
- How factors vary by role, and region.
- We will also perform clustering to find important characteristics/traits of champions which would be tied back as an input to the predictive model enabling more accurate results.

Such a model will be beneficial to the league game-playing community, especially professional players and teams that rely on game analyses.

Initial research for the project showed that there are no publicly available models that try to predict the outcome of matches for different champions. The predictive model developed in this project will be available to use for further research, such as for a live game predictor.

### Data Understanding:

To understand the data attributes we utlized information available through the RIOT developers [documentation](https://developer.riotgames.com/docs/lol#general_game-constants), and our knowledge of the game.

Our initial dataset has thirteen columns as described below.

- P_MATCH_ID - Has three values (Region, Match_id, and Role of each player)
- GOLDEARNED - Gold earned by each player            
- TOTAL MINION SKILLED - Number of minions killed
- WIN - Boolean value, True if the player’s team won the game otherwise False.                     
- KILLS - Total number of kills                    
- ASSISTS - Total number of assists by the player                   
- DEATHS - Number of times each player died in a game                      
- CHAMPION - Champion name
- VISIONSCORE - Post game stat that indicates how much vision a player has influenced in the game
- PUUID - PUUID of the player                    
- TOTAL DAMAGE DEALT TO CHAMPIONS - Damage dealt
- SUMMONER NAME - Summoner name       
- GAME VERSION - Patch Number

### Data Preparation:
The collected data needed to be preprocessed to get efficient data useful for analysis and modeling.

#### Handling missing and inconsistent values:

The dataset had few records with missing and inconsistent values. These records were dropped. Since our dataset is very large, the dropped records will not impact our analysis.

#### Feature Splitting:
The attribute P_MATCH_ID had three different relevant attributes i.e, Region, Match_ID, Role. These three attributes were extracted and appended to the data as new columns.

#### Handling unnecessary attributes:
We had a few unnecessary columns in our data. These were dropped to get a more compact dataset.

#### Exploratory Data Analysis:
We performed exploratory data analysis on our dataset in context of the relationship between the domain and the problem statement. EDA helped us to understand our data better as we plotted many interactive graphs on our dataset and found the relationship between the columns in our data.

