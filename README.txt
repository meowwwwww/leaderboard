Nguyen Phuong Nhu [A0142829Y] [BT3103 Semester 1, AY 2016/17]
Individual Assignment
=============================================================

SNAKES & LADDERS 
Software Requirement Specification

1. Original requirement Specifications
- The application supports exactly 4 players
- there will be availability of snakes and ladders
- at any one time, no 2 players have identical scores

2. Expanded specifications

#1 User have to registered/ login to play the game
Rationale: as mentioned in the gdoc, without the user login, insert into my PlayerList somehow creates duplicates of players with same attributes but different IDs. I tried to ask my group mates and look online but to no avail. However, when inserted under a user, everything works fine. So will stick to that for now.

#2 Game Rules + Do you know session next to the game play
Rationale: clarify the rule of this game since it is different from the usual snake and ladders, till to the no identical scores specification. Do you know just to makes the interface more informative. These 2 sessions are grouped together under 1 portion of the page to distinguish itself from the game play, thus makes easier for user to identify where they are (law of proximity&law of similarity)

#3 addPlayerForm disappear when exactly 4 players are in
#4 lists of snakes and ladders available in leaderboard.js file
#5 Do not allow identical scores in any cases, even in the case where player hit a snake or ladder
i.e if the player hit a snakehead and there is already somebody at the bottom of the snake, he will remain at the snake head
Similarly for ladder

3. Functional requirements
3.1 For Users:
#1 Register using email and password
#2 Login using email and password
#3 Add player until reach exactly 4 players
#4 Able to see the game rules while playing the game
#5 See which player is currently playing
#6 see explanations for each player’s score for the turn
i.e A has hit a snake at[score]. Therefore, A’s new score will be [newscore]
#7 Start a new game when current game has finished, with a new sets of players

3.2 For Players:
#1 See his score in comparison with other players in the table
#2 Check if it is his turn by seeing whether the token is next to his name
#3 Roll the dice
#4 Roll the dice again if got a 6
#5 Notified if he hit a snake
#6 Notified if he hit a ladder
#7 Notified if he got duplicate score
#8 Notified if he overshot 100
#9 Notified if he won

4. Future improvements (if time and professor permits)
- Register using Username instead of email
- Add “remove player” function
- Record history of games played
**if possible, remove User altogether

================================================================
5. Issues:
- 2 different users have identical Id: do not know how to solve yet. Therefore, for now, only 1 user can play at a time
