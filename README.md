# Snake-Game
Introduction

This is a simple console-based Snake Game written in C. The game follows the traditional rules of Snake, where the player navigates a snake around the screen, eating food to grow in length while avoiding collisions with the walls and itself.

Features

Classic snake movement using arrow keys.

Randomly generated food that increases the snake's length.

Score tracking.

Multiple lives (default: 3 lives per game).

Game-over conditions when the snake collides with itself or the boundaries.

Record keeping of player scores in a file.

Requirements

Windows OS (due to the use of conio.h and windows.h libraries).

A C compiler such as GCC (MinGW for Windows).

Installation

Clone this repository:

git clone https://github.com/yourusername/snake-game.git

Navigate to the project directory:

cd snake-game

Compile the program using GCC:

gcc snake_game_project.c -o snake_game.exe

Run the executable:

./snake_game.exe

How to Play

Use Arrow Keys to control the snake:

UP (↑): Move Up

DOWN (↓): Move Down

LEFT (←): Move Left

RIGHT (→): Move Right

The objective is to eat the food (denoted as 'F') to grow the snake and increase the score.

If the snake collides with the boundary or itself, a life is lost.

The game ends when all lives are exhausted.

Press ESC at any time to exit the game.

Game Controls

Key

Action

↑

Move Up

↓

Move Down

←

Move Left

→

Move Right

ESC

Exit the Game

Code Structure

The game consists of the following functions:

Move() - Handles snake movement and direction changes.

Food() - Generates food at random locations.

Score() - Keeps track of the player's score.

ExitGame() - Checks collision conditions and handles game-over scenarios.

Boarder() - Draws the game boundary.

record() - Saves player records to a file.

Known Issues

The game uses windows.h and conio.h, which are not compatible with Linux/MacOS.

The snake movement could be smoother with non-blocking key inputs.

The screen refresh rate can be improved for better gameplay experience.

Future Improvements

Porting to Linux/MacOS with cross-platform libraries.

Adding a graphical interface using SDL or OpenGL.

Implementing difficulty levels and speed variations
