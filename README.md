# 2.5D-Raycasting-in-C

Basic Idea: the map is a 2D square grid consisting of integer numbers, a 0 is an empty space, anything of positive value is a wall. 
The player sends out rays (where the name raycasting comes) from his field of view. These rays will walk a straight path in our 2D grid and send us a signal when they meet a wall.
Using the distance from the player to the wall met by the ray, we can draw on screen a column of pixels that represent the portion of wall hit by the ray.

The loop is really simple:
-Ray starts from player position
-if wall is hit by ray stop
-else let the ray continue
Once we stop the loop we take the distance and draw the wall with the correct height.
