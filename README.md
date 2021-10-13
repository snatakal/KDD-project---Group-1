# KDD-project - Group-1

### Team Members:
1) Tarun Ravada
2) Vishwath Kamalanathan
3) Swetha Natakala Ramakumar
4) Adithi Macherla

### Project Description:
#### Introduction
League of Legends commonly referred to as League is a highly popular Multiplayer online battle arena game.
The game annually hosts the League World Championship, which has one of the largest prize pools in e-sports. As such there are high stakes involved for the participating teams, sponsors of teams, and the viewers. Teams spend a lot of time analyzing different team compositions, matchups, and strategies to maximize their chances of winning each match.

Every match of League has many factors that affect the outcome of the match. Some examples of these factors are: the playable character (champion) being played, the number of enemy kills a player had, the amount of gold a player earned, etc.
Data analytics is used to understand the relationships between these factors so that teams can prioritize and adapt to the different changes that each match brings about. 

#### Research Question
This project will take a look at how in-game factors such as gold earned, vision score, and creep score affect the outcome of the game. The data will be analyzed to identify important trends that may be invisible to simple statistical analysis. The collected information regarding important features and trends will be used to develop a predictive model that can predict the outcome of a game given some initial match data.

Such a model will be beneficial to the league game-playing community, especially professional players and teams that rely on game analyses.

Services that summarize the performance of champions in different roles and matchups currently exist for League. However, initial research for the project showed that there are no publicly available models that try to predict the outcome of matches for different champions. The predictive model developed in this project will be available to use for further research, such as for a live game predictor. 

#### Data
The initial data source for this project is a large data set of 1v1 matchup information of players playing League at the Master rank level.
The [dataset](https://www.kaggle.com/jasperan/league-of-legends-1v1-matchups-results) was obtained from Kaggle. 
Additional game data will be obtained from League servers using the Riot Games [API](https://developer.riotgames.com/)

### CRISP-DM Process:
We have undergone these steps as part of CRISP-DM:
1) Research Phase
2) Initial Data Exploration

### Future Work
This project focuses on identifying trends in the game using data from past matches. The findings of this analysis can be used to develop applications for live game analytics.   