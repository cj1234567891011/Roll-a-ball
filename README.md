# Roll-a-ball
This is an assignment for my Game Development class in University. I follow a Unity tutorial called Roll-a-ball and then add one more level and a couple more features.
I had never built a game before or worked with a tool like Unity, but I have found it easy and fun to build this game and learn about the foundations of game development.

The main goal of the game is to build this plane where a ball is rolling around controlled by the player. To win, the ball must collect several yellow objects lying around without being caught by the enemy, a moving orange rectangle that follows the player’s every step. The most important basic concepts I learned from this tutorial are the notion of a Game object, what are Prefabs, scripts, materials, the importance of lighting and color for the player’s experience. The attention to detail makes all the difference.

For me, the hardships began once I had to make a connection between what I was seeing in the game and the code I was writing on the scripts, because I was not really visualizing how what happened in the game could be decided by whatever I inserted in the script. However, after writing a couple of functions on the script, everything became much more clearer. 
After finishing the tutorial, I added as asked one more level and some more extra features. After collecting all the objects without being caught by the enemy, the player ascends to a second level where there are two enemies, one is like the enemy from level one, and a red enemy that just randomly spawns several times in some area of the game. The extra features I added are the following:

1- Since the player can technically fall from outside the area of the game, in case that happens, a text box is shown that says “You can’t fly” while the player “falls” and the game restarts. To do so, I created this plane that is positioned underneath the game area, the "Death Zone". It acts as a trigger and everytime the player falls, it displays the text, waits for 2 seconds and restarts the game.
2- After collecting all of the collectible objects on the first level, the player needs to catch a special purple jewel to get to the second level. After the player has collected all the 13 yellow collectibles, the purple jewel only shows up in the game area.  To do so, I created a jewel object that upon being collected by the player it triggers the LevelUp function that transports the Player into the second level.
3- The players need to catch all collectibles before “night comes”, or else they lose. To do so, a function "NightTimeIsHere" where after 60 seconds into the game, the light intensity is set to 0 and a text is displyed to the user right before the game is restarted.

This was a good game to build for those who are completely new to game development. 

