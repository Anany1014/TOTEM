# TOTEM - The Chess Bot ♟️

**TOTEM** is a full-featured, 100% offline chess engine and GUI built with Python and Pygame. It offers a professional-grade experience ranging from casual play with real-time assistance to grandmaster-level calculation for tournament analysis.

---

## 🌟 Key Features

* **Adaptive ELO Slider:** Scale the engine's strength from **400 (Beginner)** to **3000+ (Magnus Tier)** with unique behavioral descriptions for each tier.
* **Move Classification:** High-precision evaluation of moves using icons for *Brilliant (!!)*, *Great (!)*, *Best (★)*, and *Blunder (??)*.
* **Assistance Mode:** Real-time hint button to suggest the optimal engine move during play.
* **Post-Game Review:** Full annotated review with statistics on move quality once the game concludes.
* **Tournament Ready:** Includes a CLI hook for processing FEN strings with a strict sub-4-second calculation limit.
* **Custom Positions:** Launch the game from any valid FEN starting position via the lobby.
* **100% Offline:** No external APIs or internet connection required for evaluation or play.

---

## 📁 Project Structure

```text
my-awesome-project/
│
├── .gitignore              # Hides secret/system files
├── README.md               # Your front-page documentation
├── LICENSE                 # Legal permissions
├── requirements.txt        # Your package versions (python-chess, pygame)
│
├── src/                    # Source code
│   ├── main.py             # Main entry point for TOTEM
│   └── utils/              # Helper functions and assets
│
├── tests/                  # Unit tests for engine logic
│   └── test_main.py
│
└── docs/                   # Extra documentation or images for the README

```

---

## 🚀 Getting Started

### Prerequisites
* Python 3.8 or higher
* Pygame
* python-chess

### Installation
1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/Anany1014/TOTEM.git](https://github.com/Anany1014/TOTEM.git)
    cd TOTEM
    ```
2.  **Install dependencies:**
    ```bash
    pip install chess pygame
    python TOTEM.py
    ```
3.  **Run the application:**
    ```bash
    python src/TOTEM.py
    ```

---

## 🕹️ How to Play
1.  **Lobby:** Adjust the bot strength, choose a time control (Blitz, Rapid, or Infinite), and select your play mode (Assistance, Independent, or Review After).
2.  **Arena:** Click a piece to see legal moves. If "Assistance Mode" is active, click **HINT** to see the engine's best recommendation.
3.  **Keyboard Shortcuts:** Press **'R'** at any time to return to the lobby and start a new game.

---

## 🛠️ Technical Details
* **Engine Algorithm:** Minimax with Alpha-Beta Pruning.
* **Evaluation:** Custom Piece-Square Tables (PST) combined with mobility and check-state scoring.
* **Move Ordering:** Implements MVV-LVA (Most Valuable Victim - Least Valuable Aggressor) for efficient tree pruning.

## 📜 License
This project is distributed under the MIT License.
