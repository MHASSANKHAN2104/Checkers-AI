
# 🧠 AI Checkers Game (Python)

A classic checkers (draughts) game implemented in Python with an AI opponent powered by the Minimax algorithm. This project includes customizable rules and supports advanced features like multi-capture king promotion.

## 🎮 Features

* **Single-player** mode vs AI (Minimax with alpha-beta pruning)
* **Classic checkers rules** with optional customization:

  * Mandatory captures
  * King promotion after multi-capture in one turn
* **Simple GUI** using `pygame`
* **Highlighting of possible moves**
* **Move history logging** for debugging and analysis

## 🧠 AI Details

* Uses the **Minimax algorithm** with optional **alpha-beta pruning**
* Adjustable search depth
* Heuristic evaluation based on:

  * Piece count and king count
  * Positional advantage
  * Capture potential

## 🛠️ Installation

1. **Clone the repository**

   ```bash
   git clone https://github.com/yourusername/ai-checkers.git
   cd ai-checkers
   ```

2. **Install dependencies**

   ```bash
   pip install pygame
   ```

3. **Run the game**

   ```bash
   python main.py
   ```

## 🧩 Game Rules

* Standard 8x8 checkers board
* Pieces can move diagonally and capture by jumping over opponent pieces
* Kings can move in both directions
* **Custom rule**: If a piece captures **two or more** opponents in one turn, it is **immediately promoted to king**

## 📁 Project Structure

```
ai-checkers/
│
├── main.py             # Entry point
├── game/               # Core game logic
│   ├── board.py        # Board representation and rules
│   ├── piece.py        # Piece logic (regular and king)
│   ├── minimax.py      # AI implementation
│   └── constants.py    # Configurable settings
└── assets/             # Images and sounds (optional)
```

## 🧪 Testing & Debugging

* Logging is provided for AI decisions and board state
* Easily adjustable `DEPTH` parameter for testing different AI levels

## 🤖 Future Improvements

* Multiplayer (local or online)
* GUI enhancements (animations, better graphics)
* AI learning (e.g., reinforcement learning instead of fixed Minimax)
* Time-limited moves and difficulty settings

