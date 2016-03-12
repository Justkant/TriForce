TriForce - Game Design
======================

Jaccarino Quentin
-----------------

Goal
----
You have to maintain the rotation of the triangle(s) for the maximum of time you can.

Players
-------
The players are assign to one or more triangle(s) which is define by colors and can touch the screen to hit the triangle

World
-----
- Timer
- Triangle(s)

Rules
-----
- The triangles are flat and start with no rotation
- The triangles rotate in 3D around their center pivot point
- The number of triangles is define by the difficulty of the game, with a maximum of 5 triangles
- The triangles are place according to the number of triangles in the world
- A color is assign to one or more triangle(s) for each player
- Triangles can have 2 colors, the first color is the color of the player assign to the triangle and the second one is black
- In multi-player, it's turn-by-turn style. Each player can only touch one triangle on his turn
- The multi-player is limited to 2 players
- If the triangle is black and the player touch it, the game is over for him
- If the triangle is not the color assign to the player who touch it, the game is over for him
- If the triangle is the color assign to the player who touch it, a force is apply to the triangle and it gain rotation force
- If the triangle rotate less than minimum speed rotation, the game is over
- The maximum and minimum speed rotation are define by the difficulty
- The force apply to a triangle can stop it, if apply in the inverse direction of the rotation
- The force apply to a triangle is calculated with the distance between the touch point and the center of the triangle multiply by a factor define by the difficulty
- If a player miss a triangle and hit the background, the game is over
- There is a real physic apply to the triangle (forces, rotations, frictions)
- Because of the physic, if the player don't touch triangle when it's rotating, it will start losing rotation speed
- In multi-player, if the second player wait until the first triangle stop, he lose
