# 🎲 Number Guessing Game in C

![Language](https://img.shields.io/badge/language-C-blue.svg)
![Status](https://img.shields.io/badge/status-Complete-green.svg)

## 📖 Overview

The **Number Guessing Game** is a command-line interface (CLI) application developed in C. It challenges users to guess a randomly generated number within a specified range, providing real-time feedback (Higher/Lower) until the correct number is guessed.

This project was built to demonstrate proficiency in core C programming concepts, including control flow, input/output handling, and random number generation logic.

## ✨ Features

* **Random Number Generation:** Uses `rand()` seeded with `time(NULL)` to ensure a unique game experience every time.
* **Input Validation:** Handles user input to ensure stability.
* **Feedback Loop:** Provides immediate "Too High" or "Too Low" hints.
* **Attempt Counter:** Tracks the number of guesses it took to win.
* **Replayability:** Allows the user to play multiple rounds without restarting the program.

## 🛠️ Tech Stack

* **Language:** C (Standard C99 or later)
* **Compiler:** GCC (GNU Compiler Collection) or Clang
* **Environment:** Cross-platform (Windows, Linux, macOS)

## 🚀 Getting Started

Follow these instructions to get a copy of the project up and running on your local machine.

### Prerequisites

You need a C compiler installed on your system.
* **Windows:** MinGW or Visual Studio.
* **Linux/macOS:** GCC is usually pre-installed. Verify by running `gcc --version` in your terminal.

### Installation & Compilation

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/saniyamir1207/random_number_guessing_game.git](https://github.com/saniyamir1207/random_number_guessing_game.git)
    cd number-guessing-game
    ```

2.  **Compile the source code:**
    For Linux/macOS:
    ```bash
    gcc main.c -o game
    ```
    For Windows:
    ```bash
    gcc main.c -o game.exe
    ```

3.  **Run the game:**
    For Linux/macOS:
    ```bash
    ./game
    ```
    For Windows:
    ```bash
    game.exe
    ```

## 🎮 How to Play

1.  Launch the application via the terminal.
2.  The system will choose a number between **1 and 100** (configurable).
3.  Type your guess and press Enter.
4.  Use the feedback hints to narrow down your next guess.
5.  Try to find the number in as few attempts as possible!

# 🧠 Technical Highlights
This project focuses on efficient memory usage and logical flow. Key implementation details include:

Standard Library Usage: Utilizes <stdlib.h> for memory/randomization and <time.h> for seeding.

Loops & Conditionals: Implements do-while loops to manage game state and if-else blocks for game logic.

Sanitization: Checks scanf return values to prevent infinite loops on invalid character inputs.

# 🔜 Future Improvements
Add difficulty levels (Easy: 1-50, Hard: 1-1000).

Implement a "Best Score" high-score system using file handling (FILE *).

Add a limited number of attempts (lives) to increase difficulty.

**Created by Saniya Mir**

### Example Output
```text
Welcome to the Number Guessing Game!
I have selected a number between 1 and 100.

Enter your guess: 50
> Too Low! Try again.

Enter your guess: 75
> Too High! Try again.

Enter your guess: 62
> Correct! You won in 3 attempts.
