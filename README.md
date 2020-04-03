# AI-OthelloGame
An AI-to-Player Othello Game with GUI on different board sizes. Uses both minimax and alpha-beta implementation with depth limit, state caching, and node ordering heuristics.

### Includes: 
- `othello gui.py`, which contains a simple graphical user interface (GUI) for Othello.
- `othello game.py`, which contains the game ”manager”. This stores the current game state and communicates with different player AIs.
- `othello shared.py`, which contains functions for computing legal moves, captured disks, and successor game states. These are shared between the game manager, the GUI and the AI players.
- `randy ai.py` , which specifies an ”AI” player (named Randy) that randomly selects a legal move.
- `agent.py`, game agent.

### Specifications
Run the Othello GUI by typing `$python3 othello gui.py -d board size -a agent.py`,
where the parameter board size is an integer that determines the dimension of the board upon which
you will play and agent.py is the game agent you would like to play against.

If you type `$python3 othello gui.py -d board size -a randy.py`, you will play against an agent that selects moves randomly, and that is named Randy. Playing a game should bring up a game window. If you play against a
game agent, you and the agent will take turns.The GUI can take also take two AI programs as command line parameters. When two AIs are specified at the command line you can watch them play against each other. 

MINIMAX: `$python3 othello gui.py -d 4 -a agent.py -m`
ALPHA-BETA: `$python3 othello gui.py -d 4 -a agent.py`
DEPTH-LIMIT: `$python3 othello gui.py -d 6 -a agent.py -l 5`
CACHING: `$python3 othello gui.py -d 6 -a agent.py -c`
NODE-ORDERING: `$python3 othello gui.py -d 8 -a agent.py -c -o.`

