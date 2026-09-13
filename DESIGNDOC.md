# Design Document

## Game Mechanics

### Topology
- Discrete 2D space
    - The world is represented by a grid;
- Semi-open world
    - The world is made up of separate open areas connected by transitions;
- Areas
    - Areas can have different shapes;
    - The boundary is defined by the outermost cells that the character can technically occupy, similar to an AABB; 

### Movement
- Simple
    - Controls: W, A, S, D;
    - The player moves on a grid in four directions;
- Kinematics
    - Position is measured in cells;
    - During movement, position is represented as a continuous value in grid cells;
    - When the player stops, the position is floored to an integer cell coordinate;

### Camera
- Follows the player's character;
- Can be constrained by the boundaries of the area;

## Graphics
- Space outside the current area is rendered as empty space;
