# TIC-TAC-TOE

This code implements a Tic-Tac-Toe game where a human player competes against an AI opponent. The game begins with the `initial_state` function, which sets up an empty 3x3 board. The `player` function determines whose turn it is based on the number of 'X's and 'O's on the board. The `actions` function identifies all possible moves by returning the coordinates of empty cells. When a move is made, the `result` function updates the board accordingly. The `winner` function checks if there's a winner by evaluating all rows, columns, and diagonals, and the `terminal` function determines if the game has ended, either through a win or a draw. The `utility` function assigns a value to the endgame states: 1 for an 'X' win, -1 for an 'O' win, and 0 for a draw.

The AI employs the `alpha_beta_pruning` algorithm to choose its moves. This algorithm uses two helper functions, `max_value` and `min_value`, to recursively evaluate potential board states, maximizing the score for 'X' and minimizing it for 'O'. The `print_board` function displays the current board state to the players. The `main` function orchestrates the game flow, starting with an empty board and alternating between the human player's and the AI's moves until the game concludes. The human player inputs their moves via row and column indices, while the AI calculates its optimal move using alpha-beta pruning. The game continues until a terminal state is reached, at which point the result is announced, indicating whether the human player won, the AI won, or if it ended in a draw.
