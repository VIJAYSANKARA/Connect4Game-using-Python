# Connect4Game-using-Python
🎮 Connect Four Game using Python (Console-Based)
This is a console-based Connect Four game built in Python. The game is a turn-based two-player competition between a human (🔵) and the computer (🔴), where players drop tokens into a 7-column, 6-row grid. The first to connect four tokens in a row—horizontally, vertically, or diagonally—wins the game.

🔧 Key Features and Functionality:
7x6 Grid Board: Represented using a 2D list, dynamically updated and printed after each move.

Player vs CPU Mode: Alternating turns between the user and a basic AI opponent using random valid moves.

Gravity Simulation: Ensures that tokens only occupy the lowest available space in a column, mimicking the real-life mechanics of Connect Four.

Win Detection: Checks for four consecutive tokens of the same type in all directions—horizontal, vertical, and both diagonals.

Input Parsing and Validation: Parses column letters (A–G) and row numbers (0–5) while validating whether the input is within bounds and follows gravity.

🧠 How it Works:
Board Setup: Initializes an empty 7-column by 6-row grid using nested lists.

User Input Handling:

Accepts coordinates like A0, C3, etc.

Converts them into list indices via the coordinateParser() function.

Gravity Logic:

Ensures that a token cannot be placed unless the cell below is occupied or the bottom row is reached.

Handled using gravityChecker().

Move Execution:

User and computer take turns.

The user inputs coordinates; the computer randomly picks a valid one.

Game Logic:

checkForWinner() scans the board after each turn for any sequence of four matching tokens.

End Condition:

When a player wins, the game announces the winner and ends.

The game board is re-printed with final token positions.

