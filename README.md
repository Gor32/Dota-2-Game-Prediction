# Dota-2-Game-Prediction
Gabe and his 9 friends enjoy playing a video game called Defence of the Ancients. This game consists of two 5-player teams fighting each other on a virtual battlefield.

Before the game starts, each player picks a virtual hero as their character from a pool of about 100 heroes. Each hero can only be picked by one player in a game. Gabe and his friends are very similar in skill-level, so the outcome of their games has some dependence on which heroes were chosen. Gabe wonders if he can predict the outcome of a game based on what heroes have been picked.

Game Data
Gabe has extensive records of past games between similar players. You can download this training data with the results of 15,000 games that Gabe has already played. You need to analyze the data to find trends about each hero. Hero names contain spaces, apostrophes, and hyphens.

The data consists of 15,000 lines, each with 10 strings and one number all seperated by commas. On each line, the first 5 strings are the heroes picked by team 1, the second 5 strings are the heroes picked by the team 2, and the number at the end is the number of the team who won.

Challenge
In each of K games, you will be given the heroes picked by each team. Using the training data, can you predict which team will win based on the heroes that they have picked? You will be scored based on how many predictions you get right. You may access the trainingdata by reading from the file "trainingdata.txt".

Input
The first line will contain a single integer K, the number of games you need to predict. This is followed by K lines containing 10 comma separated strings of the 10 chosen heroes.

Output
For each game, output the number (1 or 2) of the team you think will win on a new line.

Constraints

1 ≤ K ≤ 3000

Sample Input
5
Spectre,Nature's Prophet,Ogre Magi,Nyx Assassin,Kunkka,Lone Druid,Windrunner,Disruptor,Juggernaut,Naga Siren
Windrunner,Medusa,Zeus,Shadow Fiend,Troll Warlord,Bounty Hunter,Pudge,Lycanthrope,Riki,Pugna
Ogre Magi,Sniper,Rubick,Lifestealer,Treant Protector,Slardar,Lion,Shadow Fiend,Weaver,Nature's Prophet
Sniper,Nyx Assassin,Lich,Axe,Necrolyte,Magnus,Juggernaut,Dazzle,Tinker,Nature's Prophet
Lina,Nature's Prophet,Chaos Knight,Gyrocopter,Invoker,Sven,Broodmother,Necrolyte,Undying,Windrunner

Sample Output
1
1
1
1
1

Scoring
Your score for this challenge will based on what percentage of your predictions are correct, according to this formula:

Score = 100 * ((#correct - #incorrect) / total)

If you are are correct for less than half the games, you will receive a score of 0. Your score will only be based on the second (hidden) test case. The sample test case is just for checking if your program is working as intended in our environment.
