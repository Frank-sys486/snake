# Snake Game 🎮

A simple **Snake Game** built using Python's `tkinter` library. The game features a classic snake gameplay experience with a clean interface and smooth controls.

## Features
- Simple and intuitive controls (keyboard-based).
- Classic snake mechanics: grow the snake by eating food, avoid collisions with walls and yourself.
- Score display and a "Game Over" screen with your final score.
- Adjustable game frame rate (currently set to 10 FPS for smooth performance).

## Demo
![Snake Game Screenshot](https://github.com/Frank-sys486/snake/blob/main/preview.png)  
*An actual screenshot of the game.*

## How to Play
1. Use the **arrow keys** or **W/A/S/D** for movement:
   - **Up / W**: Move up
   - **Down / S**: Move down
   - **Left / A**: Move left
   - **Right / D**: Move right
2. The objective is to eat the red food blocks and grow your snake.
3. Avoid colliding with the edges of the screen or your own body.
4. The game ends if a collision occurs.

## Installation

### Prerequisites
- Python 3.x installed on your system.
- The `tkinter` module (comes pre-installed with most Python distributions).

### Steps
1. Clone this repository to your local machine:
   ```bash
   git clone https://github.com/your-username/snake-game.git
   ```
2. Navigate to the project directory:
   ```bash
   cd snake-game
   ```
3. Run the game:
   ```bash
   python main.py
   ```

## Code Overview
- **Game Board**: A 25x25 grid where each tile is 25x25 pixels.
- **Snake**: Starts as a single block and grows with each food item consumed.
- **Food**: Randomly spawns on the grid, and the player must navigate the snake to consume it.
- **Game Logic**: Handles movement, collisions, score tracking, and game-over conditions.

### Key Components
- `Tile` class: Represents a single grid tile, used for both the snake and the food.
- `move()`: Updates the position of the snake and handles collisions.
- `draw()`: Handles rendering the game elements (snake, food, score, etc.).
- `change_direction()`: Changes the snake's direction based on user input.

## Customization
- **Change Grid Size**: Modify the `ROWS`, `COLS`, or `TILE_SIZE` variables in `main.py` for a different game board size.
- **Speed Adjustment**: Update the delay in `window.after(100, draw)` to make the game faster or slower.

## Contribution
Contributions are welcome! If you want to enhance this project, feel free to fork the repository and submit a pull request.

### Suggestions for Future Features:
- Add sound effects.
- Implement multiple levels or difficulty settings.
- Add a pause and resume feature.

## License
This project is licensed under the [MIT License](LICENSE).

## Acknowledgments
This project was inspired by the classic Snake game. Developed with love using Python and `tkinter`. 🎉
