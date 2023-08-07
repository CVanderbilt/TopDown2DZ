# TopDown2DZ - 2D Top-Down Zombie Assault Game

![TopDown2DZ Banner](https://example.com/topdown2dz_banner.png)

TopDown2DZ is a thrilling 2D top-down game inspired by SAS Zombie Assault 2. In this action-packed game, players face hordes of zombies in waves of increasing difficulty. Your mission is to survive, strategize, and eliminate the undead threat.

## A* Algorithm and Dynamic Enemy Following Logic

One of the standout features of TopDown2DZ is its custom implementation of the A* algorithm for enemy movement. The A* algorithm enables intelligent pathfinding for enemies, making them actively follow players across the map.

What sets this implementation apart is the dynamic logic that allows enemies to follow different players or targets depending on their distance. Each enemy utilizes the A* algorithm to find the most efficient path towards its designated target.

### Flow Field for Efficient Pathfinding

To achieve smooth movement and efficient navigation, a grid of nodes is generated. Each node detects whether it falls within an obstacle, a window, or open space, influencing the cost associated with traversing that node.

These nodes are then used to compute a flow field, starting from the player's location and propagating values to adjacent nodes. This flow field facilitates reaching all reachable nodes from the source node, creating an organized path for the enemies to follow.

## Multi-Grid System for Optimized Layouts

To optimize the layout of the map, TopDown2DZ employs a multi-grid system. Different zones can have separate grids with varying sizes, and some nodes act as common connectors between these zones.

This approach avoids the need for using a single large grid with many unused nodes, reducing computational overhead. Additionally, this system enables the creation of stairs, allowing players to traverse between different floors of the map seamlessly.

![Flow Field and Multi-Grid System](https://example.com/flow_field_and_multi_grid.gif)

## Diverse Enemy Types and Weapons

TopDown2DZ offers a variety of enemy types, each with its unique abilities and challenges. Players must strategize to counter different enemy behaviors and strengths effectively.

As for the players, they have access to a range of weapons to defend against the undead horde. The arsenal includes pistols, SMGs, assault rifles, sniper rifles, and even a missile launcher with splash damage!

![Different Enemy Types](https://example.com/enemy_types.png)
![Weapons Selection](https://example.com/weapons_selection.gif)

## Chalk Painted Weapons and Interactive Elements

Taking inspiration from SAS Zombie Assault 2, the game features chalk painted weapons on the floor. Players can interact with these weapons and spend in-game currency to acquire them, providing a dynamic and engaging gameplay mechanic.

Moreover, certain sections of the map can be blocked with grey sprites, representing the top of buildings when viewed from above. Players can interact with doors and spend in-game money to unlock these blocked zones.

![Interactive Chalk Painted Weapons](https://example.com/chalk_painted_weapons.gif)
![Interactive Doors and Unlocking Zones](https://example.com/interactive_doors.gif)

## Multiplayer Mode for Cooperative Play

TopDown2DZ is evolving into a multiplayer experience, thanks to Unity's Network Manager. This multiplayer feature allows multiple players to join forces in the same game, collaborating to survive the relentless waves of zombies.

![Multiplayer Mode](https://example.com/multiplayer_mode.gif)
