# TIC-TAC-TOE-GAME
The Tic Tac Toe game is a Python-based interactive version of the classic two-player game. It features single-player mode with a computer opponent, robust winner detection, and a visually appealing interface.

# Game Rules
1. The game is played on a 3x3 grid.

2. Players take turns to mark a square with either "X" or "O."

3. You play as "X."

4. The computer plays as "O."

5. The objective is to align three of your marks in a horizontal, vertical, or diagonal row.

6. The game ends in one of three ways:
- One player aligns three marks and wins.
- The grid is filled, resulting in a tie.
- The player or computer forfeits (in-app termination).

# Developer Information
This game is developed by: 

Taanya Tapke and Ishaan Dhawan

# Algorithms Used

Winner Detection:

- Iterates through all possible winning combinations using the winners array.

- Checks whether all three positions in a combination are marked by the same player.

Computer AI for Moves (Rule-Based Approach):

- Winning Move: Attempts to win by completing a row, column, or diagonal.
- Blocking Move: Prevents the player from winning by filling a potential row, column, or diagonal.
- Strategic Moves:
Takes the center square if available.
Selects corners or edges as fallback moves, ensuring optimal gameplay.

# Game Flow

Initialization:

- A 3x3 grid is set up with blank squares.
- Images for blank cells, "X," and "O" are preloaded for display.
  
Player Turn:

- The player clicks on a square, marking it with "X."
- The game checks if the player has won after the move.
  
Computer Turn:

- The computer evaluates possible moves using predefined rules.
- Executes the optimal move and updates the grid.
- The game checks if the computer has won after its move.
  
End of Game:

- If a player wins, a winning screen is displayed with a highlighted line.
- In the event of a tie, a "Tie Game" screen is shown.

# UI Components

Grid:

- A 3x3 matrix of clickable squares, each displaying the state: blank, "X," or "O."

Graphics:
- Custom images for "X," "O," and blank states.
- Winning screens for both "X" and "O."

Dynamic Updates:
- Squares update dynamically based on player and computer moves.
- Winning combinations are highlighted with a line.

# Technologies Used

1. Python
2. Pygame (for game graphics and interaction)
3. Rule-Based AI (for computer moves)

# Key Code Component

Square Class:

- Represents each cell in the grid.
- Handles updates to the visual state and interactions.

Game Logic:
- Detects winning conditions and manages the turn-based flow.

Computer AI:
- Implements logic for determining optimal moves.

Graphics and Display:
- Uses Pygame to load, scale, and render images and animations.

Endgame Handling:
- Displays winning or tie screens and halts further input.
