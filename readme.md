# Tic Tac Toe with Tkinter GUI

## Project Overview
My goal with this project was to create a tic-tac-toe game in Python. For the game interface, I used the Tkinter GUI tool kit, which comes in the standard Python installation.

The tic-tac-toe game is for two players. One player plays X and the other plays O. The players take turns placing their marks on a grid of three-by-three cells. If a given player gets three marks in a row horizontally, vertically, or diagonally, then that player wins the game. The game will be tied if no one gets three in a row by the time all the cells are marked.

To implement the rules, the following game components were included into the program:

- The game’s board mapped by a class called TicTacToeBoard;
- The game’s logic, managed by a class called TicTacToeGame.

The game board works as a mix between view and controller in a model-view-controller design. To build the board, I used a Tkinter window represented by an instance of the tkinter.Tk class. This window has have two main components:

- Top display: Shows information about the game’s status;
- Grid of cells: Represents previous moves and available spaces or cells.

Game display is created using a tkinter.Label widget, which allows to display text and images.

For the grid of cells, I used a series of tkinter.Button widgets arranged in a grid. When a player clicks one of these buttons, the game logic will run to process the player’s move and determine whether there’s a winner.

The game logic works as the model, which manages the data, logic, and rules of the game.
___

## To run the program:

With python 3, install tkinter module using brew manager:

```
brew install python-tk
```

In the project folder create a config.py file and set up the project's parameters similar to this example:

```
from players import Player

BOARD_SIZE = 3
DEFAULT_PLAYERS = (
    Player(label='X', color='blue'),
    Player(label='O', color='green'),
)
```

In the project's directory run:

```
python tic_tac_toe.py
```

Enjoy :v:
