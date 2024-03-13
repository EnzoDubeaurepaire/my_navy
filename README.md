# my_navy - Battleship Game using Signals

## Overview
This project is a Battleship game implemented in C, designed to be played between two terminals using signals. The game was developed as a 3-week project by a team of two people.

### Team Members
- [Edgar Brunet](https://github.com/edgarbnt)
- [Enzo Dubeaurepaire](https://github.com/EnzoDubeaurepaire)

## Features
- **Two-Player Gameplay**: The game allows two players to play against each other, each using their own terminal.
- **Signal-Based Communication**: Signals are used for inter-process communication between the two players.
- **Grid-based Gameplay**: Players place their ships on a grid and take turns firing at each other's ships until one player wins.

## Requirements
- C compiler (e.g., GCC)
- Unix-like operating system supporting signals (e.g., Linux)

## How to Play
1. **Compile the Code**: Compile the code using the provided Makefile or your preferred method.
   ```bash
   make
   ```
2. **Run the Game**: Run the compiled executable in two separate terminals, one for each player.
   ```bash
   ./my_navy [path to player1 ships]
   ./my_navy [id of player1] [path to player2 ships]
   ```
   the files with the players' ships must each contain 4 lines (`ship size` `ship first position` `ship last position`), for a total of 4 ship (size must be one of each : 2, 3, 4, 5)
3. **Gameplay**: Follow the on-screen instructions to take turns firing at your opponent's grid.
4. **Winning the Game**: The game continues until one player successfully sinks all of their opponent's ships.
