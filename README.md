# TicTacToe# **Tic-Tac-Toe Game in Java**  

## **Introduction**  
The Tic-Tac-Toe game is a **turn-based strategy game** where two players take turns marking spaces in a **3×3 grid**. This Java implementation features a **human player** competing against an **AI opponent**. The game continues until a player wins by aligning their marks in a **row, column, or diagonal**, or the game results in a **draw** when the board is full.

---

## **Game Features**  

### ✅ **1. Game Board Management**  
- The game board is represented using a **3×3 character array** (`char[][] board`).
- Initially, all cells are set to **empty (' ')**.
- A method (`dispBoard()`) visually represents the grid in a user-friendly format.

### ✅ **2. Player System**  
The game consists of two players:  
- **Human Player** (`HumanPlayer` class) → Allows manual input for moves.  
- **AI Player** (`AiPlayer` class) → Randomly picks an available move.

### ✅ **3. Move Validation**  
- Players can only place marks in **empty** and **valid** positions on the board.
- The system prevents **overwriting existing marks** or placing marks **outside the grid**.

### ✅ **4. Win & Draw Detection**  
- **Winning Conditions**:
  - A player wins if they get **three consecutive marks** in a **row, column, or diagonal**.
- **Draw Condition**:
  - If the board is full and no player has won, the game ends in a **draw**.

### ✅ **5. Game Loop & Turn Management**  
- The game starts with the **human player** (`'X'`), followed by the **AI player** (`'O'`).
- The turn alternates after each valid move.
- The game ends when a player **wins** or the board is **full (draw)**.

---

## **How the Game Works**  
1. The **game board is initialized** (all cells are empty).  
2. Players **take turns** placing their marks.  
3. After each move, the game **checks for a winner** or a draw.  
4. The game **continues until a win condition or draw is met**.  
5. If a player wins, their name is displayed. Otherwise, a **"Game is draw"** message appears.  

---

## **Example Game Flow**  
```
Likith turn
Enter the row and col: 0 0
-------------
| X |   |   |  
-------------
|   |   |   |  
-------------
|   |   |   |  
-------------

AI turn
-------------
| X |   |   |  
-------------
|   | O |   |  
-------------
|   |   |   |  
-------------

Likith turn
...
Likith has won!
```

---

## **Future Improvements**
🔹 **Smarter AI**: Implement **Minimax Algorithm** for better AI decisions.  
🔹 **GUI Version**: Use **Java Swing** or **JavaFX** for a graphical interface.  
🔹 **Online Multiplayer**: Connect via **Sockets** for remote play.  

This game provides a solid foundation for further development and enhancements. 🚀
