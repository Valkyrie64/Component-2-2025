# Component 2 Manual
This manual will explain how the component works and how it will be used in the final prototype

## Player
The player is on the left hand side and fires a bullet when the "E" key is pressed. This will be the same input in the final prototype.

## Enemy
The enemy is on the right hand side of the screen and will be destroyed when the bullet intersects with it. This interaction is performed with the OnTriggerEnter() function and the collision.CompareTag() function.

## Bullet
The bullet is a prefab that is created using the Instantiate() function, and continously moves based on its own script. It is tagged as "Bullet" which is used for the interaction when it hits the enemy. It is destroyed both when colliding with an enemy and also when it goes off-screen, using the IsVisible() function.

## Implementation
In the final prototype, the enemies will be spawning in on screen based on a random interval timer, and will have the ability to shoot at the player. There will also be a change made to the bullet interaction, as there will be both "enemy" bullets and "player" bullets, and therefore the only one type of bullet should affect the player or enemy respectively.
