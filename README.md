# CPSC 481 Project 1 - State Space Search for Pacman
## Authors
- RJ Andaya
- Andrew Dinh
- Fanghua Gu
- Bijaya Shrestha

## Introduction (Algorithm Used)
In he search.py file, depth-first search(DFS) algorithm was implemented in the depthFirstSearch function. This depth-first search algorithm avoids visting any visited states by using stack(), and breadth-first search algorithm in breadthFirstSearch function is using Queue() as list to keep track current state. The base case of dfs algorithm is first tracking if the current state is goal state, if yes it returns the legalAction. If no then the dfs algorithm will visit the childs of current state and continue this branch until it reaches the goal state. The base case of bfs is to track if the currrent state is the goal state, if yes then return the legalAction. If no then the bfs algorithm will visit next state in the same level until it reaches the goal state.

## Setup and Installation
Download the code with implementation, open up the pacman.py file and execute the file by entering the execute command. The pacman will be efficiently navigated in the maze with highlighter path. 

## Sample Invocation
By running out the following commands, the pacman would be able to explore the maze with the hightlighter path. The brighter color represents the earlier path or exploration of the maze. 

commands for depth-first search for solving the tinyMaze, mediumMaze and bigMaze:
python pacman.py -l tinyMaze -p SearchAgent
python pacman.py -l mediumMaze -p SearchAgent
python pacman.py -l bigMaze -z .5 -p SearchAgent

commands for breadth-first search for solving the mediumMaze and bigMaze:
python pacman.py -l mediumMaze -p SearchAgent -a fn=bfs
python pacman.py -l bigMaze -p SearchAgent -a fn=bfs -z .5


## Bugs
N/A

## Issues
N/A
