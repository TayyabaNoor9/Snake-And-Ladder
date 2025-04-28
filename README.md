# Snake and Ladder Game

## Overview
The **Snake and Ladder Game** is a classic board game implemented in C++ that allows two players to compete against each other in a race to reach the finish line at square 100. The game integrates visual elements using the console, along with dice rolling mechanics to determine player movement.

## Features
- **Two-player Mode:** Players take turns rolling a die to advance on the board.
- **Snake and Ladder Mechanics:** Players can land on snakes that send them backward or ladders that advance them forward.
- **Scoreboard:** Displays player scores and the effects of landing on snakes and ladders.
- **Dynamic Console Display:** Uses console graphics for an engaging user experience.
- **Game Rules Display:** Provides instructions on how to play the game.

## How to Play
1. **Starting the Game:**
   - The game begins by displaying rules and instructions.
   - Players need to roll a six to start their journey on the board.

2. **Rolling the Dice:**
   - Players take turns rolling a six-sided die.
   - The outcome determines how many spaces they move forward on the board.

3. **Landing on Snakes or Ladders:**
   - Landing on a square with a snake sends the player back to a lower square.
   - Landing on a square with a ladder advances the player to a higher square.

4. **Winning the Game:**
   - The first player to reach square 100 wins the game.

## Technologies Used
- **Programming Language:** C++
- **Libraries:** Standard libraries for console input/output, random number generation, and time handling.

## Code Structure

```
SnakeAndLadder/
│
├── main.cpp               # Main game logic and execution
│
└── README.md              # Project documentation
```

## How to Run the Game

1. Ensure you have a C++ compiler installed (e.g., g++, Visual Studio).
   
2. Compile the code:

   ```bash
   g++ main.cpp -o SnakeAndLadder
   ```

3. Run the compiled program:

   ```bash
   ./SnakeAndLadder
   ```

4. Follow the on-screen instructions to play the game.

## Game Logic Overview

- **gotoRowCol(int rpos, int cpos):** Moves the console cursor to specified coordinates.
- **Print_Box(int rdim, int cdim, char b):** Draws the game board box.
- **Print_in_Box(int rdim, int cdim, int num):** Fills the game board with numbers.
- **print_snake_ladder():** Displays the snake and ladder graphics on the board.
- **scoreboard():** Displays the current score and positions of players.
- **snake_ladder1() / snake_ladder2():** Updates player positions based on snakes and ladders.
- **Dise1() / Dise2():** Handles dice rolling for each player.
- **rollingdise():** Manages the main game loop and player turns.
- **display():** Shows the game rules.

## Limitations
- The game is currently limited to two players.
- The board is fixed in size and does not support additional features like player profiles or saving progress.
