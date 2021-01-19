# Tic-Tac-Toe Game

A terminal-based tic-tac-toe game, utilising the minimax algorithm, alpha-beta pruning and cutoff. The AI-player uses the minimax algorithm to take decisions on each turn and the human player will get a recommendation before each move.

# Well, what is the *Minimax Algorithm*?

Minimax is a kind of backtracking algorithm that is used in decision making and game theory to find the optimal move for a player. The two players involved in a game (which utilizes the minimax algorithm) are called maximizer and minimizer. The maximizer tries to get the highest score possible while the minimizer tries to do the opposite and get the lowest score possible. <br> [Note: It is possible to have more than two players. For example, the minimax algorithm can also be implemented in a game of Connect Four] <br>
Every board state has a value associated with it. In a given state if the maximizer has upper hand then, the score of the board will tend to be some positive value. If the minimizer has the upper hand in that board state then it will tend to be some negative value. The values of the board are calculated by some heuristics which are unique for every type of game. <br>
### Taking the example of the tic-tac-toe game, <br>
**Tie** represents a null or balanced state between the maximizer and the minimizer. <br>
**Victory** represents the presence of either a positive or negative score. <br>
<hr>
Alpha-Beta pruning and cutoff are used to speed up the search time for the minimax algorithm. Alpha-Beta pruning means that we can ignore searching through nodes that never will be chosen given the information we already have (both players are assumed to play optimally). <br>
Cutoff means that we can use a fast heuristic* evaluation algorithm when we have reached a certain depth in the minimax search. Cutoff is used in the early phases of a game when the number of possible plays is very high. <br>

*Heuristic: The objective of a heuristic is to produce a solution in a reasonable time frame that is good enough for solving the problem at hand. This solution may not be the best of all the solutions to this problem, or it may simply approximate the exact solution. But it is still valuable because finding it does not require a prohibitively long time. Heuristics may produce results by themselves, or they may be used in conjunction with optimization algorithms to improve their efficiency (e.g., they may be used to generate good seed values). For more information, visit [Wikipedia's page on heuristics](https://en.wikipedia.org/wiki/Heuristic_(computer_science)#Definition_and_motivation).*


# To clone

`$ git clone https://github.com/AdityaBhattacharya1/tic-tac-toe`

### Install dependencies:

`pip install -r requirements.txt`

# To run

`cd` into the directory and run: <br>
`python main.py`
