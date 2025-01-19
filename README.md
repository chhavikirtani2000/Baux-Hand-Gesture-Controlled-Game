# Baux
Python-Arduino based interactive game.
Team Members-
Dibya Gautam, Chhavi Kirtani, Shubhi Singhal, Chhavi Munjal 


In the generation of plenty of computer games which are played using mouse and keyboard, we have made a game controlled by hand gestures. This game stimulates the hand movement of the user.

We are taking user interaction in the game with the help of two sensors. One (on the right side of the box) is controlling the left and right movement of the player and the other (on the front of the box) is controlling the action performed by the player, whether attraction or destruction. The colour of the player keeps on changing and it needs to attract the coin of the same colour as that of it and it needs to destroy different coloured coins. 


RULES
When the distance of the hand is within 15 cm from the right sensor, the player moves left. When it is between 15 cm and 40 cm, the player moves right. If the distance is greater than 40 cm, the remains at its current position. Similarly, for the front sensor, when the distance is within 15 cm, it attracts the coin; for distance between 15 cm and 40 cm, it destroys the coin, and for distance greater than 40 cm, coins are neither destroyed nor attracted.


WORKING
We made use of ultrasonic sensors to capture the user input based on the position of his hand in front of the sensor. Based on the above mentioned distance values, we print out certain message to Arduino serial monitor, which is in turn read and processed using python to make changes according to the user interaction into the game.


SCORING
On attracting the desired colour, the score gets incremented by 1. On destroying the different colour, the score as well as the lives left remains same. And if the coin gets missed, 1 life is lost. In total, we have 30 lives at the start of the game. 

To win the game, we need to attract 3 desired coins of the same colour consecutively.
		

