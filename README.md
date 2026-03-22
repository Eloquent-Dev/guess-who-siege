# R6S Guess Who? ![Version](https://img.shields.io/badge/version-1.0-red)

A web-based, local multiplayer deduction game inspired by the classic board game "Guess Who?", fully themed around the operators of Rainbow Six Siege.

## 🎮 How to Play
This is designed as a pass-the-device (or shared screen) game for two players.

1. **Player 1:** Clicks "Assign Secret Operator" to roll a random target.
2. **Player 1:** Memorizes the operator, then clicks "Hide Details".
3. **Player 2:** Takes over and asks Yes/No questions to deduce Player 1's operator (e.g., *"Is your operator a Defender?"*, *"Does your operator have a shield?"*).
4. **Player 2:** Clicks on operator cards on the main grid to eliminate them based on the answers.
5. When Player 2 thinks they know the answer, they make their final guess!

## ✨ Features
* **Complete Roster:** Includes 77 operators updated through Year 11 (including crossovers like Solid Snake).
* **Authentic UI:** Edge-to-edge operator portraits with overlapping UI badges, mimicking the official Rainbow Six website.
* **Smart Fallbacks:** The code automatically attempts to load high-quality `.avif` images first, and seamlessly falls back to standard `.png` files if they are missing.
* **Role Tabs:** Easily swap between Attackers and Defenders to manage the massive roster.

## 📁 Installation & Setup
Because this project uses copyrighted Ubisoft image assets, the image files are not included in the base code. You must provide your own images and place them in the correct folder structure.

Your project directory must look exactly like this:

```text
/r6s-guess-who
│
├── index.html        (The main game file)
├── README.md         (This file)
│
└── /assets
    ├── /images       (Operator portraits go here)
    │   ├── sledge.png
    │   ├── ash.avif
    │   └── ...
    │
    └── /badges       (Operator icons go here)
        ├── sledge.png
        ├── ash.avif
        └── ...