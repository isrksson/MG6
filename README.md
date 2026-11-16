# MG6

1. The entire for loop will finish within a single frame before the `Update()` method finishes. The engine will not move on to the render the next frame until everything is finished executing in the `Update()` method. If a for loop takes a really long time to finish, it will lag the game.
2. The logic of turning off the player's collider allows the player to not interact with the wall/ground collider, allowing the player to move through the boundaries. This can result in glitches of the player going out of bounds or clipping inside platforms/wall.
