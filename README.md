# 2048 Game 

This project is a Python implementation of the popular **2048 game** using the `pygame` library. The game consists of a 4 x 4 grid where tiles with powers of 2 merge when they collide, with the goal of reaching the **2048 tile** or higher.

![2048](https://github.com/0maaz-01/2048/blob/main/1.png)

## Features
- A functional 4 x 4 grid for tiles.
- Smooth tile movement and merging animation.
- Keyboard controls for movement (arrow keys and `W`, `A`, `S`, `D`).
- Automatic spawning of new tiles after each move.
- Game over detection when no more moves are possible.

## Prerequisites
Before running the game, ensure the following are installed on your system:
- Python 3.7 or higher
- `pygame` library

To install `pygame`, use:
```bash
pip install pygame
```

## How to Run
1. Save the script in a file named `2048_game.py`.
2. Open a terminal and navigate to the directory containing the file.
3. Run the script using:
   ```bash
   python 2048_game.py
   ```

## Controls
- **Arrow Keys** or **W, A, S, D**: Move tiles up, down, left, or right.
- **ESC** or close button: Exit the game.

## How to Play
1. The game starts with two tiles (value `2`) randomly placed on the grid.
2. Use the controls to move tiles. When two tiles with the same value collide, they merge into a single tile with a value equal to their sum.
3. After each move, a new tile (value `2` or `4`) will spawn at a random empty location.
4. The game ends when no moves are possible.
5. Try to create the `2048` tile to win, but you can keep playing for higher scores!

## Code Overview
### Constants
- **Grid Dimensions**: The game uses a 4 x 4 grid defined by `ROWS` and `COLS`.
- **Tile Colors**: A dictionary maps tile values to their respective colors.
- **Font**: Text rendering uses the `pygame.font.SysFont`.

### Classes
- **`Tile`**: Represents an individual tile on the grid, managing its value, position, and rendering.

### Functions
- **`draw_grid`**: Draws the grid lines.
- **`draw`**: Renders the grid and all tiles on the screen.
- **`generate_tiles`**: Initializes the grid with two starting tiles.
- **`move_tiles`**: Handles tile movement, merging, and the addition of new tiles.
- **`get_random_pos`**: Determines a random position for spawning new tiles.

### Main Loop
- The `main()` function manages the game loop, handling events, drawing the screen, and checking for game termination.

## Customization
### Change Colors or Styles
Modify the `Tile.COLORS` dictionary to change the tile colors.

### Adjust Grid Size
To modify the grid size, update `ROWS` and `COLS` accordingly. Ensure other constants like `RECT_HEIGHT` and `RECT_WIDTH` adjust dynamically.

### Difficulty
Adjust the chance of spawning higher-value tiles by modifying the `random.choice([2, 4])` in the `end_move` function.

## License 
This project is licensed under the MIT License - https://github.com/0maaz-01/2048/blob/main/LICENSE
---
## [Visit My Website](https://www.maazverse.com/)
