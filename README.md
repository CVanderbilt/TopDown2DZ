# TopDown2DZ - Work-in-Progress 2D Top-Down Zombie Assault Game

TopDown2DZ is an exciting work-in-progress 2D top-down game inspired by SAS Zombie Assault 2. In this ongoing project, players will face hordes of zombies in waves of increasing difficulty. Your mission will be to survive, strategize, and eliminate the undead threat.

## Flow Field and Dynamic Enemy Following Logic

One of the standout features of TopDown2DZ is its innovative approach to enemy movement. Instead of using the A* algorithm to get the path from each enemy to the nearest player, the game employs A* from the players to create a flow field that guides the enemies' movements.

### Flow Field for Efficient Pathfinding

To achieve smooth movement and efficient navigation, a grid of nodes will be generated. Each node will detect whether it falls within an obstacle, a window, or open space, influencing the cost associated with traversing that node.

The grid setup is straightforward. We simply position it, choose the row and column count, and adjust the node spacing. Greater spacing reduces node count, but also decreases obstacle detection accuracy and path generation precision.
![Grid setup](https://media1.giphy.com/media/v1.Y2lkPTc5MGI3NjExdGFzbnRwMHJ0N2RmbzNnODFndWJ3ZGZnOHhpZm92ZWFwM2YyOWJncyZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/rdd3GGr4ivuEEFdjuZ/giphy.gif)

Starting from the player's location, A* will be performed to compute a flow field that propagates values to adjacent nodes. This flow field will guide the enemies' movements by providing directional information for efficient pathfinding towards the players.

## Multi-Grid System for Optimized Layouts

To optimize the layout of the map, TopDown2DZ will employ a multi-grid system. Different zones can have separate grids with varying sizes, and some nodes will act as common connectors between these zones.

This approach will avoid the need for using a single large grid with many unused nodes, reducing computational overhead. Additionally, this system will enable the creation of stairs, allowing players to traverse between different floors of the map seamlessly.

![Flow Field and Multi-Grid System](https://media4.giphy.com/media/v1.Y2lkPTc5MGI3NjExczRta3JtZXMzNWwyMmZoeGV6aTh0MGhtbzR5Z3duMjUycGRleGFudCZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/1K8uABjxp9kJ4WQYxd/giphy.gif)

![Stairs](https://media1.giphy.com/media/v1.Y2lkPTc5MGI3NjExOTBiaHl2MXZmejU2NjNudWliaXFsMWpqajlzZmZxODQ3NnBoenoyeSZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/6DHYBdLKi5ErXRBg3z/giphy.gif)

![Stairs 2](https://media3.giphy.com/media/v1.Y2lkPTc5MGI3NjExbDl6M3JpOHlmbThnam4yNm5kMHY2cTh3ZHhvNHRkZG1pdXRrOHIzbyZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/yHmbFvLgksUkiBXhno/giphy.gif)

## Diverse Enemy Types and Weapons

TopDown2DZ will offer a variety of enemy types, each with its unique abilities and challenges. Players must strategize to counter different enemy behaviors and strengths effectively.

As for the players, they will have access to a range of weapons to defend against the undead horde. The arsenal will include pistols, SMGs, assault rifles, sniper rifles, and even a missile launcher with splash damage!

Enemies:
|||
|-----------------------|------------------------|
| Big zombie: lots of health and lots of damage ![GIF 1](https://media3.giphy.com/media/v1.Y2lkPTc5MGI3NjExb243MmlxcTBiNHVjamhiNDAyeG9odnV4ajBmbnltaDViaXBkN3RhYyZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/kHv6Fzr8lizzldXSVt/giphy.gif)| Fast zombie: low health + faster than regular ![GIF 2](https://media3.giphy.com/media/v1.Y2lkPTc5MGI3NjExYjdqaGVveGNnOHFoamQ1MDRza201aTk0cXBqaXVzajNvZnhxdHJ4MSZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/0eJ3gLeSv2Ba6O6JhT/giphy.gif)|
| Gray zombie: faster and stronger than regular ![GIF 3](https://media4.giphy.com/media/v1.Y2lkPTc5MGI3NjExd2JpNDc4YmRmNGphbGN2dWkzN25xbXdjNzNpZGl1YW4xNTZxcWx3ZSZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/32JVUV4ULuGZTMxmk7/giphy.gif)| Regular zombie: basic enemy unit, not special ![GIF 4](https://media1.giphy.com/media/v1.Y2lkPTc5MGI3NjExbWdoaWg3MjFhaHp4eGFkZXpjY3pkNjlxNDl4NTU0dmNlc2p3aHkwbCZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/pn8jcnHFNEgq4EwrtW/giphy.gif)|

## Chalk Painted Weapons and Interactive Elements

Taking inspiration from SAS Zombie Assault 2, the game will feature chalk painted weapons on the floor. Players can interact with these weapons and spend in-game currency to acquire them, providing a dynamic and engaging gameplay mechanic.

Moreover, certain sections of the map can be blocked with grey sprites, representing the top of buildings when viewed from above. Players can interact with doors and spend in-game money to unlock these blocked zones.

![Interactions, doors, windows, chalk](https://media1.giphy.com/media/v1.Y2lkPTc5MGI3NjExc2ZqYjJ1MHd4djdxZ2xtbDJsMGhnY211N2J3bWdvM245aDVmNnZqeSZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/Es9DtdjKappwH9KlGj/giphy.gif)

## Multiplayer Mode for Cooperative Play (Upcoming Feature)

TopDown2DZ is currently in development, and we are actively working on implementing a multiplayer feature using Unity's Network Manager. This upcoming feature will allow multiple players to join forces in the same game, collaborating to survive the relentless waves of zombies.

## Note: Ongoing Development

Please note that TopDown2DZ is still a work-in-progress and not a published game. The project is continually evolving, and we are excited to bring new features, content, and improvements as development progresses.

Stay tuned for updates and follow the project's development journey!
