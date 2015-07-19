# 2048
APCS Final Project of 2048! :)

### MainScene Class
\n Requirements: The MainScene class manages all the game logistics. This means that the score, options, pausing, ending, and restarting the game are all managed in the MainScene. 
The Functional Specifications: To create and manage the MainScene, the following functionality must be provided:
Keeps track of the current status of the game, most easily said by tracking the score.
The score is managed like so: <ul>
<li> Only tiles that are the same value can be added together (and thus the same color value)
*Score is calculated by the number of moves made
*In order to win the game: You must reach the highest number possible. In standard games, the highest is 2^11, or 2048. 
*To lose the game: No moves are left, meaning that there are no empty tiles left in the 4 by 4 grid. 
*Gives the option to reset the game when there are no moves left, meaning that the game will have to begin from score 0. 

Grid Class
Requirements
The Grid class is the entire background and playing field for the game. This means that all movement and interaction between the tiles is accounted for in the Grid class. 
The Functional Specifications
To create and manage the Grid Class, the following functionality must be provided.
Stores all the Tiles that are currently on the Grid in a LinkedList
Is a 4x4 grid at the start of the game
Tiles that collide are moved in the following way:
either up, down, left, or right
tiles move all the way to the direction they are pressed to with only the walls or other tiles to stop their movement
when a tile moves from one “filled” grid square to another one OR collides, the previous square is “empty”
the game begins with 2 filled tiles of the lowest color and numerical value
Waits for player input of a key press: 
Each player input is a press of an arrow key. 
With the press of an arrow key, update the board to exhibit above described behavior. 

Tile Class
Requirements
The Tile class stores all the information on a single tile. This means that the color, value, location, and more of the tile are all stored in the tile class. When collisions occur on the grid, the data from the Tile class is the data that is affected. 
The Functional Specifications
To create and manage the Tile class, the following functionality must be provided:
Stores and handles the information for each tile in the Grid.
Location
Value
To see what is the current state of the Tile, refer to the Grid class. 
When a tile collides with another tile, three things about it are changed:
the value is added together
the color shades are altered
the location of the tile changes
Only two tiles are allowed to collide in a single turn. 
