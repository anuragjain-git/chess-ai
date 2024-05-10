# Chess

A simple chess game implemented in Python using the Pygame library.
It features a basic AI that calculates the optimal move by peeking DEPTH moves ahead. The AI assesses positions and scores only.

![Untitled video - Made with Clipchamp](https://github.com/anuragjain-git/chess/assets/98457054/bfdea7e5-502b-4852-a2c9-115ea32e45da)

## Introduction

This is a basic implementation of a chess game with a graphical user interface. The game allows two players to make moves on a standard chessboard. Additionally, there is an AI opponent that uses negamax algorithm, alpha beta pruining for move selection.

## Features

- **Graphical User Interface:**
  - The game features a user-friendly graphical interface developed using the Pygame library.

- **Two-player Mode:**
  - Play against a friend in human vs. human gameplay. Enjoy the classic chess experience with two human players.

- **AI Opponent:**
  - Challenge yourself against an AI opponent equipped with the negamax algorithm and alpha-beta pruning. The AI has options to make valid moves, providing a single-player chess experience.

- **Checkmate, Stalemate, and Legal Moves:**
  - The game checks for conditions such as checkmate, stalemate, and legal moves, ensuring a fair and rule-compliant gameplay experience.

- **Advanced Chess Mechanics:**
  - Supports advanced chess mechanics, including pawn promotion, en passant, and castling for a more strategic and engaging experience.

- **Undo and Reset Board:**
  - Press Z for undo, R for reset

- **Variety of Chess Boards:**
  - Enjoy playing on different chess board colors, adding a personalized touch to your gaming experience.

- **Immersive Sounds and Images:**
  - Enhance your gaming experience with multiple piece move or capture sounds.

## En Pasant

In chess, the en passant rule allows a pawn to capture an opponent's pawn that has moved two squares forward from its starting position. The capturing pawn moves to the square immediately beyond the captured pawn. Here's how it works:

1. **Initial Position:**:

   <img src="https://github.com/anuragjain-git/chess/assets/98457054/1b92957b-1126-4771-8ffb-e3fe7a77b4ca" alt="Chessboard" width="400"/>

2. **Opponent's Move:**

   <img src="https://github.com/anuragjain-git/chess/assets/98457054/bba26e9f-86b2-421b-99b0-a0e7c73a49d9" alt="Chessboard" width="400"/>

3. **En Passant Capture:**

    <img src="https://github.com/anuragjain-git/chess/assets/98457054/d77b5e0c-cd11-41e2-86d1-687267586c63" alt="Chessboard" width="400"/>

## Pawn Promotion:

In chess, pawn promotion occurs when a pawn reaches the eighth rank. The pawn can be promoted to any other chess piece (except a king). Here's how it works:

1. **Reach the Eighth Rank**:
    
   <img src="https://github.com/anuragjain-git/chess/assets/98457054/9d33967c-6d19-478c-bb23-8737e4325510" alt="Chessboard" width="400"/>

2. **Select the Promotion Piece**:

   <img src="https://github.com/anuragjain-git/chess/assets/98457054/42fc5e0e-f782-4d55-a454-37c13dd39ffa" alt="Chessboard" width="400"/>

## How to Play

1. Clone the repository to your local machine.
   
2. Install the required dependencies.
   
   ```bash
   pip install pygame

3. Run the `main.py` script to start the game.

   ```bash
   python main.py

**Using Visual Studio Code:**

- Open Visual Studio Code.
   
- Click on "File" -> "Open Folder" and select the cloned directory.
   
- Open the integrated terminal in Visual Studio Code.

- Run the following command to start the game:

    ```python
    python main.py
    
## Controls

The controls for the chess game are designed to be intuitive and user-friendly.

- **Selecting a Piece:**
  - Click on the chess piece you want to move. The selected piece will be highlighted to indicate that it's ready for a move.
  - If AI is thinking you can click on AI piece to see all possible moves.

- **Moving a Piece:**
  - After selecting a piece, the legal moves for that piece will be highlighted on the chessboard.
  - Click on one of the highlighted squares to move the selected piece to that position.

The game will automatically handle the rules of chess, including legal moves, capturing opponent pieces, pawn promotion, en passant, and castling.

## Installation

1. Clone the repository:
   
   ```bash
   git clone https://github.com/anuragjain-git/chess-bot.git
   
2. Navigate to the project directory:
   
   ```bash
   cd chess
   
3. Install dependencies:
   
   ```bash
   pip install -r requirements.txt
   
4. Run the game:
   
   ```bash
   python main.py

## Settings for AI

### Human vs Human Gameplay:

If you want to play a game where both players are human:

- Open the `main.py` file and modify the following lines:

   ```python
   SET_WHITE_AS_BOT = False
   SET_BLACK_AS_BOT = False

- To flip the board, go to `engine.py` and set:

   ```python
    self.playerWantsToPlayAsBlack = False

### AI Gameplay:

If you want to play a game with the AI:

- Open the `main.py` file and modify the following lines:

   ```python
   SET_WHITE_AS_BOT = True
   SET_BLACK_AS_BOT = False

- To flip the board, go to `engine.py` and set:

   ```python
    self.playerWantsToPlayAsBlack = False

### DEPTH:

The `DEPTH` setting determines how many moves ahead the AI will consider during its search for the best move. A higher depth generally results in a stronger AI, but it also requires more computational resources.

This emphasizes the recommendation to keep the `DEPTH` value at 4 or lower for a balance between AI strength and computational efficiency.

If you want to modify DEPTH:

- Open the `chessAi.py` file and modify the following lines:

  ```python
   DEPTH = 3

### Acknowledgments:

Special thanks to the Pygame library for providing a straightforward and effective means to develop graphical applications in Python. The ease of use and versatility of Pygame greatly contributed to the creation of this chess engine.

**Contributions and Feedback:**
This project is open to contributions from the community. If you have ideas, want to report issues, or suggest improvements, feel free to contribute on GitHub. Your input is valuable in enhancing the overall quality and functionality of this chess engine.

