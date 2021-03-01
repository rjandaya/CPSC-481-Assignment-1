# CPSC 481 Project 1 - State Space Search for Pacman
## Authors
- RJ Andaya
- Andrew Dinh
- Fanghua Gu
- Bijaya Shrestha

## Introduction (Algorithm Used)
In the search.py file, the Depth-First Search(DFS) algorithm was implemented in the depthFirstSearch function. This depth-first search algorithm avoids visting any visited states by using a stack, and the breadth-first search algorithm in the breadthFirstSearch function uses a queue to keep track of the current state. The base case of the DFS algorithm is to track if the current state is a goal state. If so, it returns a list of legal actions. Otherwise, the DFS algorithm will visit the children of the current state and continue this branch until it reaches the goal state. The base case of BFS is to track if the currrent state is the goal state. If so, return the list of legal actions. Otherwise, the BFS algorithm will visit next state in the same level until it reaches the goal state.

## Setup and Installation
Download the project code, and execute the project by executing one of the commands listed in the command.txt in Command Prompt(Windows) or Terminal(macOS/Linux). Pacman will navigate efficienlty in the maze. 

## Sample Invocation
By executing the following commands, Pacman will be able to explore the maze with the hightlighted path.

Commands for depth-first search for solving the tinyMaze, mediumMaze and bigMaze:<br />
	python pacman.py -l tinyMaze -p SearchAgent<br />
        python pacman.py -l mediumMaze -p SearchAgent<br />
	python pacman.py -l bigMaze -z .5 -p SearchAgent<br />


Commands for breadth-first search for solving the mediumMaze and bigMaze:<br />
	python pacman.py -l mediumMaze -p SearchAgent -a fn=bfs<br />
	python pacman.py -l bigMaze -p SearchAgent -a fn=bfs -z .5<br />


## Bugs
N/A

## Issues
N/A
