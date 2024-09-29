# Snake Game by @evitabarboza

This is a classic Snake game implemented using Python's `turtle` graphics library. The player controls the snake's movement to eat food, and each time the snake eats food, it grows longer. The game ends if the snake runs into the screen boundaries or itself.

## Features
- A grid-based movement system using `turtle`.
- Snake grows longer each time it eats food.
- Randomly placed food items within the screen boundaries.
- Game tracks the current score and high score.
- Collision detection with the borders and the snake's own body.

## Getting Started

### Prerequisites
- Python 3.x
- The `turtle` module, which comes pre-installed with Python.

### Installation
1. Ensure you have Python 3.x installed on your system.
2. Clone this repository or download the game script.
3. Open a terminal or command prompt, and navigate to the folder where the script is saved.

### Running the Game
Run the following command in your terminal:
```bash
python snake_game.py
```

The game window will open, and you can begin playing.

### Controls
- **W**: Move Up
- **A**: Move Left
- **S**: Move Down
- **D**: Move Right

### Game Over Condition
The game ends if:
- The snake touches the borders of the window.
- The snake runs into its own body.

When the game ends, the snake resets to the center of the screen, and your score is reset to zero. However, the high score is saved until the game is closed.

## Code Overview

### Main Components:
- **Snake Head:** The main player-controlled object, which moves based on keyboard input.
- **Food:** A red dot that appears randomly on the screen, and the snake must eat it to grow.
- **Segments:** Each time the snake eats food, it grows longer, with new segments being added to the body.
- **Scoreboard:** The game tracks the player's current score and the high score, updating it dynamically.

### Important Functions:
- **move()**: Handles the movement of the snake based on its direction.
- **go_up(), go_down(), go_left(), go_right()**: Control functions tied to the keyboard for snake movement.
- **place_food()**: Randomly places the food on the screen, ensuring it doesn't overlap with the snake's body.
- **Collision Detection**: Ensures that the game ends when the snake collides with the borders or its own body.

## Future Improvements
- Add levels of difficulty.
- Implement sound effects.
- Add graphical improvements like a start screen and game-over screen.
- Introduce obstacles to make the game more challenging.

## License
This project is open-source and available under the [MIT License](https://opensource.org/licenses/MIT).
