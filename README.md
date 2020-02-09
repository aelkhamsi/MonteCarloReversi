# Monte Carlo Tree Search for the game Reversi

## Commands
To play a game between two agents using the Monte Carlo search tree algorithm as a decision strategy:

    python3 localGame1.py

To play a game between a Monte Carlo player and an Alpha Beta player:

    python3 localGame2.py
    
## Description of the files

* **MonteCarlo.py**: in this file, we've implemented two classes:
  * **MonteCarloNode**: Represents a node in the search tree. The attributes of this class include the parent node, the children nodes, the number of times the node have been visited and the UBC1 score of the node.
  * **MonteCarloTree**: Represents the Monte Carlo tree. Includes methods for searching the optimal move where the current state of the board is the tree's root. (**treeWalk** & **randomWalk**)
  
* **monteCarloPlayer.py**: Represents a player based on the Monte Carlo Tree Search for its decision making with Iterative deepening (1 second for each move). 

* **alphaBetaPlayer.py**: Represents a player based on the alpha beta algorithm for its decision making with Iterative deepening (1 second for each move).

* **localGame1.py**: Play a game between two Monte Carlo players.
* **localGame2.py**: Play a game confronting a Monte Carlo player (BLACK) against an Alpha Beta player (WHITE)
## Results

The Monte carlo and the alpha beta players were confronted in **10 matches**. </br>
The score was **8** wins for Monte Carlo, against **2** wins for Alpha Beta
