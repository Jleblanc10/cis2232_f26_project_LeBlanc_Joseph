# CIS2232 / CIS2250 Business Topic

# This document will provide details on the specific business need that the web application in CIS2232 and mobile application in CIS2250 will be built to serve.  This is a custom topic that you think up.  For the topic that you come up with, you will be the business representative.  Another student will be the developer for this topic.  There are to be between 6-10 fields to be captured so the scope is limited.  

# As a part of the project, there must be a calculation involved.  This could be a cost, an average or some other accumulation based on several of the input fields but some type of calculation to be described.   It can be anything really but something that would take some manipulation / calculations based on the input fields.  You may make up some details to allow a calculation. 

# In groups of three – interview each other to find something that each person is interested in.  This can be related to a hobby that the student has, a prior job that they had, or a sport that they like.  Brainstorm the topic to come up with a little information system that can be used as a topic for second year courses.  

# Project Group

# BA / Business Client	Steven

# Developer	Joseph

# Project Manager / QA	Kay

# 

# Project Title

# 

# World Cup Player Effectiveness Ratings

# 

# 

# Project Base Color

# 

# Forest Green

# 

# 

#  

# Description (300 words)

# 

# This application allows users to enter a player from the FIFA 2026 World Cup tournament and their stats. It will take those stats and create a player effectiveness score for each player. The stats that will be tracked are:

# 

# Player Name

# Country

# Position

# Minutes Played

# Goals

# Assists

# Defensive Actions (Tackles + Blocks + Interceptions)

# Yellow Cards

# Red Cards

# Player Effectiveness

# 

# A weight value must be given for goals, assists, defensive actions, yellow cards and red cards (as shown in the example calculation below). 

# 

# The number goals and assists entered by the user will be multiplied by their weighted value then added together. This value is then divided by the minutes played then multiplied by 90 to get a per-90-minute rate stat for offensive contributions. The same will be done for defensive contributions. 

# 

# The number of yellow and red cards entered by the user will be multiplied by their weighted value then added together. They will also be divided by the minutes played then multiplied by 90 to get the per-90-minute rate stat for penalties.

# 

# The sum of the offensive contributions, defensive contributions and penalties will be the player effectiveness score. 

# 

# Fields

# Name	Data Type	Description

# id	int	Unique identifier for database table

# playerName	String	Player’s name

# country	String	The country the player plays for

# position	String	The position the player plays (DEF, MID, FWD)

# minutesPlayed	int	Total minutes the player played in the tournament

# goals	int	The number of goals the player scored in the tournament

# assists	int	

# defensiveActions	int	The sum of the player’s tackles, blocks and interceptions in the tournament

# yellowCards	int	The number of yellow cards the player received

# redCards	int	The number of red cards the player received

# playerEffectiveness	Double	The calculated score of the players overall effectiveness for the tournament

# &#x09;	

# Calculation

# &#x20;For example,

# 

# GOALS\_WEIGHT = 1.0

# ASSISTS\_WEIGHT = 0.75

# DEFENSE\_WEIGHT = 0.5

# YELLOW\_CARDS\_WEIGHT = 0.5

# RED\_CARDS\_WEIGHT = 2.0

# 

# double getOffensiveContribution = ((goals \* 1.0) + (assists \* 0.75) / minutesPlayed) \* 90

# double getDefensiveContribution = ((defensiveActions)\*0.5) / minutesPlayed) \* 90

# double getPenalties = ((yellowCards \* 0.5) + (redCards \* 2.0) / minutesPlayed) \* 90

# 

# playerEffectiveness = offense + defense – penalty

# 

# 

# Repository

# Once the document is completed, move the details a repository that you create.  The developer creates the repository for the topic that they will be coding.  Add the other two project group members to the repository.  Add this document to the repository (Commit/Push).  The description is to be added to the readme file of the Bitbucket repository.



