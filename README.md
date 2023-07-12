Game Winner Prediction - Pubg Dataset

1.Introduction
PUBG stands for Player's Unkown Battlegrounds, which is a multiplayer game that is available on various platforms which are Windows, Android, IOS, etc. The game features different modes, the three different modes are Classic, Arcade, and EvoGround. In classic, the player will be provided with different maps that range from Erangel, Miramar, Sanhok, and Vikendi. In the arcade mode, there are War, Mini-Zone, Quick Match, and Sniper Training. There are 555 Million Players worldwide playing PUBG on all different platforms, with this huge number comes the ranking difficulty. The basic match of Battle Royal consists of 100 people playing a match with only 1 Winner (who can have Chicken Dinner). Ranking these players on basis of different attributes becomes difficult as there is a possibility of some players with more than one similar ranking.

2.Problem Statement
1.Prepare a complete data analysis report on the given data

2.Create a predictive model which is an attempt to predict the win probability of the Pubg match and to look at the important factors affecting the win probability of the pubg game.

Domain Analysis
Id - Each player have a unique ID.

groupId - Each group have a unique ID.

matchId - Each match have a unique ID.

assists - Number of enemy players this player damaged that were killed by teammates.

boosts - Number of boost items used.

damageDealt - Total damage dealt. Note: Self inflicted damage is subtracted.

DBNOs - Number of enemy players knocked.

headshotKills - Number of enemy players killed with headshots.

heals - Number of healing items used.

killPlace - Ranking in match of number of enemy players killed.

killPoints - Kills-based external ranking of player. (Think of this as an Elo ranking where only kills matter.) If there is a value other than -1 in rankPoints, then any 0 in killPoints should be treated as a “None”.

kills - Number of enemy players killed.

killStreaks - Max number of enemy players killed in a short amount of time.

longestKill - Longest distance between player and player killed at time of death. This may be misleading, as downing a player and driving away may lead to a large longestKill stat.

matchDuration - Time taken to complete a single match.

matchType - String identifying the game mode that the data comes from. The standard modes are “solo”, “duo”, “squad”, “solo-fpp”, duo-fpp”, and “squad-fpp”; other modes are from events or custom matches.

maxPlace - Worst placement we have data for in the match. This may not match with numGroups, as sometimes the data skips over placements.

rankPoints - Elo-like ranking of player. This ranking is inconsistent and is being deprecated in the API’s next version, so use with caution. Value of -1 takes place of “None”.

revives - Number of times this player revived teammates.

rideDistance - Total distance traveled in vehicles measured in meters.

roadKills - Number of kills while in a vehicle.

swimDistance - Total distance traveled by swimming measured in meters.

teamKills - Number of times this player killed a teammate.

vehicleDestroys - Number of vehicles destroyed.

walkDistance - Total distance traveled on foot measured in meters.

weaponsAcquired - Number of weapons picked up.

winPoints - Win-based external ranking of player. (Think of this as an Elo ranking where only winning matters.) If there is a value other than -1 in rankPoints, then any 0 in winPoints should be treated as a “None”.

winPlacePerc - The target of prediction. This is a percentile winning placement, where 1 corresponds to 1st place, and 0 corresponds to last place in the match. It is calculated off of maxPlace, not numGroups, so it is possible to have missing chunks in a match.
