# Game-of-life

# Overview
- The Game of Life is a cellular automaton devised by mathematician John Conway. It is a zero-player game, meaning that its evolution is determined by its initial state, with no further input from humans. The game consists of a grid of cells, and the state of each cell 
- evolves based on a set of rules.

# Features
- Customizable Initial State: The initial state of the game can be loaded from a file named "gol.txt."
- User-Defined Cycles: The user can specify the number of cycles the game should run, simulating the evolution of the cellular automaton.
- Display with Ncurses: The game is displayed using the Ncurses library, providing a simple and interactive text-based interface.


# How to Run

- Compile the program using a C compiler (e.g., gcc).
gcc game_of_life.c -o game_of_life -lncurses

. Run the compiled executable.
./game_of_life

# File Structure
- game_of_life.c: The main source code file containing the implementation of the Game of Life.
- gol.txt: A sample file containing the initial state of the cellular automaton. The file format represents 0s and 1s on each line, defining the initial state of each cell.

# Rules
- The evolution of each cell is determined by the following rules:
- Any live cell with fewer than two live neighbors dies, as if by underpopulation.
- Any live cell with two or three live neighbors lives on to the next generation.
- Any live cell with more than three live neighbors dies, as if by overpopulation.
- Any dead cell with exactly three live neighbors becomes a live cell, as if by reproduction.

# Dependencies
- Ncurses Library: The project utilizes the Ncurses library for creating a text-based user interface.
