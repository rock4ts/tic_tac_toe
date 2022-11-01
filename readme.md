### A tic-tac-toe game built with Python and Tkinter.

**To run the program:**
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