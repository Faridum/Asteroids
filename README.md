# Asteroids Game

A modern implementation of the classic **Asteroids** arcade game built with **Python** and **Pygame** as part of my Boot.dev learning journey. While following the course, I also extended the project with several gameplay improvements and refactored parts of the code to make it cleaner and easier to maintain.

## Features

* Player movement and rotation
* Projectile shooting system
* Asteroid spawning and splitting
* Score system
* Lives system
* Player respawn
* Temporary invincibility after respawning
* Automatic removal of nearby asteroids after respawn
* Screen wrapping
* Clean, modular project structure

## Technologies Used

* Python 3
* Pygame
* Git

## Project Structure

```text
.
├── asteroid.py
├── asteroidfield.py
├── circleshape.py
├── constants.py
├── logger.py
├── main.py
├── player.py
├── shot.py
└── ...
```

## Installation

Clone the repository:

```bash
git clone <repository-url>
cd <repository-folder>
```

Create a virtual environment (recommended):

```bash
python -m venv .venv
```

Activate the virtual environment.

### Linux / macOS

```bash
source .venv/bin/activate
```

### Windows

```bash
.venv\Scripts\activate
```

Install the required dependency:

```bash
pip install pygame
```

## Running the Game

Run the game with:

```bash
python main.py
```

If you are using **uv**, you can also run:

```bash
uv run main.py
```

## Controls

| Key       | Action        |
| --------- | ------------- |
| **W**     | Move Forward  |
| **S**     | Move Backward |
| **A**     | Rotate Left   |
| **D**     | Rotate Right  |
| **Space** | Shoot         |

## Gameplay

* Destroy asteroids to earn points.
* Each destroyed asteroid awards **10 points**.
* The player starts with **3 lives**.
* After losing a life, the player:

  * Respawns at the center of the screen.
  * Receives temporary invincibility.
  * Clears nearby asteroids to avoid immediate collisions.
* The game ends when all lives are lost.

## License

This project is intended for learning and educational purposes.
