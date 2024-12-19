# 🎯 Peg Reversal Game

## Project Overview

The **Peg Reversal Game** is a challenging single-player board game where the objective is to flip all the pegs on a '+' shaped board to white. Starting with one white peg and all others black, players must strategically flip pegs while adhering to the rules of adjacency. The game provides an engaging puzzle-solving experience that requires planning and logical thinking.

## How to Play

1. The board is shaped like a '+' with pegs, initially set with one white peg, and all others black.
2. A player can flip a black peg to white only if at least one adjacent peg (up, down, left, or right) is already white.
3. The game is won when **all pegs on the board are flipped to white**.
4. Explore all possible moves and strategize to reach the winning state efficiently.

---

## Features

- 🛠️ **Board Initialization**  
  Generates the initial board state, ensuring one white peg and the rest black, based on a user-specified position.
  
- ✅ **Move Validation**  
  Ensures moves adhere to the rules of adjacency and legality within the current board configuration.
  
- 🏆 **Goal Check**  
  Automatically evaluates the board to determine if the winning condition (all white pegs) is achieved.
  
- 🔍 **Explore Possible States**  
  Provides a comprehensive list of all unique next board states, helping players visualize their options.
  
---

## Technologies

- 🏗️ **Haskell**: Leveraging the power of functional programming for clarity and efficiency.  
- 🧩 **Functional Programming Paradigms**: Employing immutability, recursion, and pure functions.  
- 🔄 **Recursion**: For seamless state transitions and board evaluations.  

---

## Functions

- **`createBoard :: Position -> Board`**  
  Initializes the board with one white peg at the given position. Returns an error for invalid positions.

- **`isValidMove :: Move -> Board -> Bool`**  
  Checks if a move is legal based on the current board state.

- **`isGoal :: Board -> Bool`**  
  Returns `True` if all pegs on the board are white, otherwise `False`.

- **`showPossibleNextStates :: Board -> [State]`**  
  Lists all possible next states from the current board configuration.
