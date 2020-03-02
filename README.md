![Imgur](https://i.imgur.com/DRLTW0j.png)

### Objective

The objective of this project is twofold: first, to use data from the 2017 & 2018 NFL seasons to predict how many yards a player will run the ball after receiving a handoff; second, to determine the most important factors in the data collected by the NFL's newly implemented Next Gen Stats system in predicting rush yardage.

### The Data

The data set was furnished by the NFL. It contains the 49 features listed below. Each row in the file corresponds to a single player's involvement in a single play. The player is assigned a unique `PlayerId`, and the play is assigned its own unique `PlayId`. Therefore, each play is comprised of 22 rows: one for each player on the field--both offense and defense. All the columns are contained in one large dataframe which is grouped by PlayId.  

The data includes game-level circumstantial features, such as weather, temperature, playing surface, location, etc.; player-level features, such as the player's name, team, number, height, weight, position, etc.; and play-level features, such as time of snap, time of handoff, down number, and yardage gained on the play (our target). The Next Gen Stats system uses chips that are embedded into the shoulder pads of each player as well as the ball to provide additional measurements that are specific to each player for each play, like the player's, orientation, distance covered and acceleration (calculated from the last 0.1 seconds of play).
   
A - acceleration in yards/second^2  
DefendersInTheBox - number of defenders lined up near the line of scrimmage, spanning the width of the offensive line   
DefensePersonnel - defensive team positional grouping  
Dir - angle of player motion (deg)  
Dis - distance traveled from prior time point, in yards  
DisplayName - player's name  
Distance - yards needed for a first down  
Down - the down (1-4)  
FieldPosition - which side of the field the play is happening on  
GameClock - time on the game clock  
GameId - a unique game identifier  
GameWeather - description of the game weather  
HomeScoreBeforePlay - home team score before play started  
HomeTeamAbbr - home team abbreviation  
Humidity - humidity  
JerseyNumber - jersey number  
Location - city where the game is being played  
NflId - a unique identifier of the player  
NflIdRusher - the NflId of the rushing player  
OffenseFormation - offense formation  
OffensePersonnel - offensive team positional grouping  
Orientation - orientation of player (deg)  
PlayDirection - direction the play is headed  
PlayerBirthDate - birth date (mm/dd/yyyy)  
PlayerCollegeName - where the player attended college  
PlayerHeight - player height (ft-in)  
PlayerWeight - player weight (lbs)  
PlayId - a unique play identifier  
Position - the player's position (the specific role on the field that they typically play)  
PossessionTeam - team with possession  
Quarter - game quarter (1-5, 5 == overtime)  
S - speed in yards/second  
Season - year of the season  
Stadium - stadium where the game is being played  
StadiumType - description of the stadium environment  
Team - home or away  
Temperature - temperature (deg F)  
TimeHandoff - UTC time of the handoff  
TimeSnap - UTC time of the snap  
Turf - description of the field surface  
VisitorScoreBeforePlay - visitor team score before play started  
VisitorTeamAbbr - visitor team abbreviation  
Week - week into the season  
WindDirection - wind direction  
WindSpeed - wind speed in miles/hour  
X - player position along the long axis of the field. See figure below.  
Y - player position along the short axis of the field. See figure below.  
YardLine - the yard line of the line of scrimmage  
Yards - the yardage gained on the play    

![image.png](attachment:image.png)  
<img src="field_diagram.png" width="800">
