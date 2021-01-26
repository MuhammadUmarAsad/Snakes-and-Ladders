# Project Title:   Snakes and Ladders by Core Four

## Group Members:

-	Muhammad Ali Usman
-	Ayesha Shamim Naime
-	Sameen Mubashar 
-	Fatima Hussain

### Short project description:

The game we developed is the traditional snake game. The main idea of the game is to gain score by eating fruits, and preventing the snake from colliding with itself, walls or obstacles.

### Features:

####	Three different levels to make the game more enjoyable
1.	An easy level with no boundaries or obstacles (free space)
2.	An intermediate level with a boundary. The snake is now confined within a specific area.
3.	A hard level with a boundary and an obstacle. The user now has to prevent the snake from colliding with the boundary and the obstacle, making it more challenging.
-	Each level has a snake different colored snake adding on to aesthetics
-	A regular fruit that increases speed and length of snake
-	A bonus fruit that provides extra score. The user has a limited time to eat as many bonus fruits as possible. 
-	Two bonus fruits that appear simultaneously: one benefits the user by decreasing the length of snake, while the other harms the user by increasing length of snake. The user has a limited time to eat one of these. The idea is to eat the beneficial fruit, while dodging the detrimental fruit.
-	A soothing music to complement user’s gaming experience

Technical Architecture:

**Our game primarily consists of four components:**
~~~
•	Snake
•	Fruit
•	Collisions
•	GUI
~~~
**Further we are using following third party libraries for our game:**
~~~
•	Random
•	Time
•	Pygame
•	OS
~~~


`Through the apt integration of these components and libraries, we have achieved the desired results. On backend a grid of 600 × 600 pixels is created for the game. This is achieved by using pygame library. Time module is used to control the frame rate of the gameplay. We are using lists within list for snake to print it on the screen where every inner list is actually part of the snake body. The movement of snake is mapped with the grid by adjusting the dimensions accordingly. Every component of the snake including the head is of dimension 30 × 30.`

`The movement of snake is divided into two types. One is user defined and other is the automatic movement of the snake. We have managed the user defined movement of the snake by specifying four keys (up, down, right ,left) for the respective movements. Further in case user wants the snake to move in a specific direction, we have managed the automatic movement in that particular direction.`

`We have controlled the random appearance of fruit on the parts of grid which are allowed for the movement of snake which is achieved by using random module. When there is collision between the fruit and the snake, which actually means that the coordinates of snake head become equal to that of the fruit, a change is made in many parameters of the game. This includes the increase in the speed of the game which is achieved by using time module.`

`Length of snake is increased by appending the already present list of snake to make game more competitive as the time goes on. Similarly score is increased and is displayed on the screen. The fruit then reappears at some random point on the grid which is not forbidden. We have created boundaries and obstacles in different levels of the game. In case of collision of snake with any of the coordinate specified as boundary and obstacle the game gets over and user is shown his score along with the high score.`

`Basically, we store the high score in a separate text file and use it in the main program to compare it with the score of users. In addition, we are making sure that the fruit does not appear on any point on grid specified for boundary, obstacle, on snake’s body or on other fruit. To make the game more interesting, we have added three kinds of bonus fruits in our game.`

`One of the fruits appears after user has eaten five normal fruits and give two additional points giving accumulatively three points to user. This type of fruit keeps appearing for specific time and user can eat it as many times he wants.` 

`Two other fruits appear after snake eats five normal fruits. One of them is beneficial and decreases the length of snake and other is disadvantageous for the user as it increases the length of the snake. Both of these appear for specific time on screen which is achieved through time module.`

`Pygame is used for the GUI of game. We have integrated images and sound effects with the game to improve the gameplay. We have also added a high score feature through which the user can see the highest points they had in all the games played. Here, the os module is used to check whether the file to save user’s high score exists or not. If it does not exist, it is created.`


#### How to run and deploy your code:

To begin with, download Python from the official website of Python: [click Me](https://www.python.org/downloads/)

Then, open command prompt (or terminal in Mac or Linux) and enter the command
*`pip install pygame`*.

`This is used to install the external module pygame.`

#### Note: Users with both Python2 and Python3 installed on their systems should type “pip3 install pygame” instead. 
Lastly, ensure all files are in the same folder. When that is done, run the file “snake.py” using python and the game will begin. For best experience, we recommend you to run the game directly from the .py using python. Users interested in development of game are welcome to use an IDE for the execution of the game. Enjoy gaming!
