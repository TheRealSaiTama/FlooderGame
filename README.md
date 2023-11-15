# Flooder

Flooder is a flood fill game built in Python with the bext module. The goal of the game is to fill the entire board with a single color tile in a limited number of moves.

## How to Play

When the game starts, you are presented with a randomly generated board with tiles of different colors. To make a move, you select one of the 6 colors, and that color will flood outward from the top left corner, replacing connected tiles of the same color. 

You have a limited number of moves to try to flood the entire board with one color. If you run out of moves, you lose. If you manage to convert the full board to a single color tile, you win!

The allowed moves are:

- R - Choose Red
- G - Choose Green 
- B - Choose Blue
- Y - Choose Yellow
- C - Choose Cyan
- P - Choose Purple

## Code Overview

The game is implemented in Python using these main functions:

- `get_new_board()` - Generates a random new board 
- `display_board()` - Prints the board with colors to the terminal 
- `ask_for_player_move()` - Gets the player's color choice for the next move
- `change_tile()` - Performs the flood fill from the top left corner
- `has_won()` - Checks if the board is all one color

The `bext` module is used for coloring the terminal output. 

The flood fill algorithm uses recursion to spread the chosen color in all four directions, replacing connected tiles of the same color.

## Installation

Requires Python 3 and the `bext` module. Install with pip:

```
pip install bext
```

Then run `flooder.py` to play!

The full code is available in [this Github repo](https://github.com/TheRealSaiTama/FlooderGame). Feel free to fork and modify!
