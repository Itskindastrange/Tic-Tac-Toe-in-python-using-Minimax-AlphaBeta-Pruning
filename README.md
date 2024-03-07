# Tic-Tac-Toe-in-python-using-Minimax-AlphaBeta-Pruning
This code implements a Tic-Tac-Toe game with a computer opponent utilizing the Alpha-Beta pruning minimax algorithm for AI decision making.
initial_state(): Initializes an empty 3x3 Tic-Tac-Toe board.
player(gameBoard): Determines whose turn it is based on the current state of the board.
actions(gameBoard): Finds all possible valid moves (empty cells) on the board.
result(gameBoard, action): Simulates the result of placing a mark ('X' or 'O') in a given cell on the board.
winner(gameBoard): Checks if the game has a winner (horizontal, vertical, or diagonal lines) or is over.
terminal(gameBoard): Determines if the game is in a finished state (win or draw).
utility(gameBoard): Assigns a score to a terminal game state: 1 for 'X' win, -1 for 'O' win, 0 for a draw.
maxVal(gameBoard, alpha, beta): Recursive function for the minimax algorithm (maximizing player, 'X'). Implements alpha-beta pruning for efficiency.
minVal(gameBoard, alpha, beta): Recursive function for the minimax algorithm (minimizing player, 'O'). Also uses alpha-beta pruning.
AlphaBetaMiniMaxAlgo(gameBoard): Determines the best move for the AI by applying minimax with alpha-beta pruning.
draw_board(gameBoard): Prints a visual representation of the board.
play(): The core game loop that handles player input, AI moves, and the overall game flow.
Game Logic

The game starts with an empty board.
The player chooses to play as 'X' or 'O'.
Players take turns placing their marks on the board.
The game checks for winning conditions after each placement.
If no winner is found and the board is full, the game ends in a draw.
The AI uses the Alpha-Beta Minimax algorithm to determine the optimal moves.
Alpha-Beta Pruning

Alpha-beta pruning is an optimization technique for the minimax algorithm.
It reduces the number of nodes explored in the game tree by discarding branches that cannot influence the final decision.
How to Use

Save the code as a Python file (e.g., tictactoe.py)
Run the code from your terminal using python tictactoe.py
Follow the prompts to play the game.
