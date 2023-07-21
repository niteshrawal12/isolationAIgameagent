# Isolation AI Game Agent

![Isolation AI Game Agent](/viz.gif) <!-- If you have a screenshot, replace the "path/to/your/game-screenshot.png" with the actual path -->

Isolation AI Game Agent is a two-player deterministic game implementing the minimax algorithm with alpha-beta pruning and Iterative Deepening Search. The game is played on a rectangular grid, similar to chess, where players alternate turns moving a single piece of Knight. Each agent can make L-shaped movements (like a knight in chess) to any open cell on the board that is 2-rows and 1-column or 2-columns and 1-row away from their current position. The objective is to block the opponent's moves until one player runs out of legal moves, making the other player the winner.

## Rules

- Players take turns moving their Knight piece on the board.
- Once a cell is occupied by a player, it becomes blocked for the rest of the game.
- Knights can move in L-shaped patterns, like in chess.
- The first player with no remaining legal moves loses, and the opponent is declared the winner.

## Technology Used

- Java
- Java Swing and AWT

## Environment Set-up

To set up the Isolation AI Game Agent environment, follow these steps:

1. Install Java JDK 8 on your system.
2. Use IDE Netbeans for Java AWT and Swing in GUI (Graphical User Interface) to design the grid layout of the Rectangular 8x8 chess board.
3. Use Image Icons of black and white knights in the resources folder.
4. Extract the ZIP file and locate the `src` folder inside with the command prompt.
5. Execute the program:
   - Use 'cd' in the command prompt to navigate to the 'src' folder.
   - Enter: `javac Isolation.java`
   - Enter: `java Isolation`

## Explanation of Algorithms

### Minimax Algorithm

The Minimax Algorithm is a popular method for adversarial search problems in a multiplayer setting. It evaluates the state of the game, where one player aims to maximize the score, and the other wants to minimize the score away from the first player. This algorithm helps calculate the best move in any given state to aid victory.

The code includes a `minimax()` method that evaluates available moves using recursion. The MAX player tries to find the best move, while the MIN player selects moves to minimize MAX's outcome.

### Alpha-Beta Pruning Algorithm

The alpha-beta pruning method is a technique to speed up the computation of the minimax algorithm. It uses an alpha and beta value to set a minimum standard to look for, allowing the algorithm to skip unnecessary paths and improve efficiency.

### Iterative Deepening Search

Iterative deepening search limits the depth of each path the algorithm explores. This helps to foresee a specified number of moves instead of endlessly calculating through irrelevant paths.

The `iterativeDeepening()` method in the code implements this technique.

## Development Process

The development process for this project involved several challenges:

- Debugging issues while creating and testing functions for the Isolation class.
- Implementing the UI using Java AWT and Swing to match project specifications.
- Designing a heuristic to improve AI moves, considering both aggressive and defensive strategies.
- Overcoming obstacles in implementing the alpha-beta pruning algorithm.
- Addressing recursive function callback challenges during the implementation of minimax, alpha-beta pruning, and Iterative Deepening Search.
  
Overall, we learned so much through this project and it was extremely fun to work on.
