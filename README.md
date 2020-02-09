# Monte Carlo Tree Search for the game Reversi

## Commands
To launch a game between two agents using the monte carlo search tree algorithm as a decision strategy:

    python3 localGame.py
    
## Description of the files

* **MonteCarlo.py**: in this file, we've implemented two classes:
  * **MonteCarloNode**: Represents a node in the search tree. The attributes of this class include the parent node, the children nodes, the number of times the node have been visited and the UBC1 score of the node.
  * **MonteCarloTree**: Represents the Monte Carlo tree. Includes methods for searching the optimal move where the current state of the board is the tree's root. (**treeWalk** & **randomWalk**)
  
* **myPlayer**: Represents a player based on the Monte Carlo Tree Search for its decision making with Iterative deepening. 
