🧠 Minesweeper AI (CS50 Project)

This project implements an AI agent that plays Minesweeper using logical reasoning and knowledge-based inference.

The AI is able to analyze the board, build knowledge about safe cells and mines, and make decisions based on that knowledge.

🚀 Features

✅ Knowledge-based AI (logical inference)

✅ Automatic deduction of safe cells and mines

✅ Subset-based inference (advanced reasoning)

✅ Random move fallback when no safe move is known

✅ Fully playable game with GUI (pygame)

🧠 How It Works

The AI represents knowledge in the form:

{cells} = count

Example:

{A, B, C} = 1

This means exactly one of these cells contains a mine.

The AI uses:

Safe detection → if count = 0 → all cells are safe

Mine detection → if count = number of cells → all are mines

Knowledge updating → removing known cells and updating counts

Subset inference:

{A, B, C} = 1  
{A, B, C, D, E} = 2  
→ {D, E} = 1
🛠️ Technologies

Python 3.11+

Pygame

Object-Oriented Programming (OOP)

Basic AI / Logic reasoning

▶️ How to Run
1. Install dependencies
pip install -r requirements.txt
2. Run the game
python runner.py
3. Play

Left click → reveal cell

Right click → mark mine

Click "AI Move" to let AI play

📁 Project Structure
minesweeper/
│
├── minesweeper.py   # Game logic + AI
├── runner.py        # GUI (pygame)
├── assets/          # Images and fonts
└── requirements.txt
⚠️ Limitations

The AI is not perfect

Sometimes it must make random moves

This reflects real-world uncertainty in AI systems

💡 What I Learned

Knowledge-based AI design

Logical inference using sets

Object-oriented programming in Python

Working with Git & GitHub

Building a complete project with UI
