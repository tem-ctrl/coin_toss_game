# coin_toss_game
 
![coin_toss_image](coin_toss.jpg) <br>
In this project, I will show how to implement a simple coin toss game in python.

## Game rules

This game is played by a single user against the computer. The player predicts the outcome of three consecutive coin tosses, for example **THH** where **H** stands for **heads** and **T** satands for **tails**. Behind the scenes, the computer makes its own prediction based on that of the user. The coin is then flipped until the last three consecutive coin tosses match either predictions. The player wins in the case his/her prediction is the one obtained, otherwise the computer wins. In either case, the player is given the chance to retry.

The `main.ypinb` contains the code for the game. <br>
More explanations can be found on [my blog here](https://www.datainsightonline.com/post/simple-apps-with-python-coin-toss-game)

## Game extension
Question: Alice and Bob are playing a game. They start by each writing down a prediction of the outcome of three consecutive coin tosses; for example, Alice might write down **(T, H, H)** and Bob might write down **(H, T, H)**. They then continue flipping a coin until the last three consecutive coin tosses match either of their predictions, and the matching prediction is the winner. <br>

Show that Bob has an advantage if, knowing Alice’s choice **(A1, A2, A3)**, he chooses **(¬A2, A1, A1)**. In other words, estimate his odds of winning and show that they are greater than Alice’s. <br>
Note: the symbol ¬  means **not**. If **A2 = H**, then **¬ A2 = T**. If **A2 = T**, then **¬ A_2 = H**. <br>


To address this exercice, Bob's odds of winning are evaluated over 10000 tries, for each possible alice's prediction and the average is evaluated to answer the question.

Find the related code in the file `extension.ypinb`.
