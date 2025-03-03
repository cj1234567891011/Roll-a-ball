# Roll-a-ball
This is an assignment for my Game Development class in University. I follow a Unity tutorial called Roll-a-ball and then add one more level and two features.

The main goal of the tutorial is to build this plane where a ball is rolling around controlled by the player. To win, the ball must collect several yellow objects lying around without being caught by the enemy, a moving orange rectangle that follows the player’s every step. After collecting all the yellow collectibles, the enemy disapeers, but the player does not level up until he collides with the purple jewel.

The initial hardships I had related to the project were the lack of experience with the tools in the Unity editor. Such difficulties disappeared once I was into the tutorial and had build some of the features. After finishing the tutorial, I added as asked one more level and some more extra features.

One of the features I added was the Death Zone. Since the player can fall from the game area, I created a plane object that is bigger and is position directly under said game area. When the player enters in contact with the Death Zone, which is set to be a trigger, it displays a message, waits for 2 seconds and restarts the game. This was a solution I found for the player falling into the unknown and not being able to get out in case of flying out of the game area. 

Another feature I added was the "Night Time". After a certain amount of time, if the player has not levelled up yet, the "night time" comes and the game restarts. It was made with the intention to cause adrenaline in the player. There is a set time (60 seconds) in which the Invoke method inside of the Start() method in the PlayerController.cs class calls a NightIsHere() method. In this method, the light intensity is set to 0, a message is displayed and the game restarts. All the other features are in the PlayerController.cs class, but this feature has its own NightTimeController.cs class because it's not connected to any player action.

The last feature I added was a special purple jewel that allows the player to level up, only after the player has collected all the 13 yellow collectibles. To do so, I created a jewel object which is a trigger. After the count gets to 13, meaning all yellow collectibles were caught, and checking if the text shown when leveling up is not active, it spawns the purple jewel in specific coordinates in the game area and destroys the enemy. Upon being collected by the player, it triggers the LevelUp() function in the PlayerController.cs class that triggers a LevelTransition() function that then transports the Player into the second level.

Finally, to create the second level, the scene was duplicated, but the game area was made smaller.

Notes: The SpawnPurpleJewel() method in the PLayerController. cs class was heavily inspired in the prompt in this website: https://discussions.unity.com/t/how-to-parent-spawned-object-from-array-solved/826062


