# 🎯 Peg Reversal Game

## Project Overview

This project implements a single-player board game where the goal is to flip all pegs on a '+' shaped board to white. The game starts with one white peg and all others black. Players can flip a black peg to white if there is at least one white peg adjacent to it (up, down, left, or right). The game is won when all pegs are white.

## Features

- 🛠️ **Board Initialization**: Generates the initial board state with one white peg and the rest black.
- ✅ **Move Validation**: Checks if a move is valid based on the current board state.
- 🏆 **Goal Check**: Determines if the board is in a winning state with all pegs white.
- 🔍 **Possible States**: Lists all unique possible board states from a given board configuration.

## Technologies

- 🏗️ Haskell
- 🧩 Functional Programming
- 🔄 Recursion

## Functions

- **`createBoard :: Position -> Board`**  
  Initializes the board with one white peg at the given position. Returns an error for invalid positions.

- **`isValidMove :: Move -> Board -> Bool`**  
  Checks if a move is legal based on the current board state.

- **`isGoal :: Board -> Bool`**  
  Returns `True` if all pegs on the board are white, otherwise `False`.

- **`showPossibleNextStates :: Board -> [State]`**  
  Lists all possible next states from the current board configuration.
