# Simon Game

This is a simple implementation of the classic **Simon** game using Qt and C++. The game challenges players to memorize and repeat an increasingly long sequence of colors.

## Features
- **Graphical User Interface (GUI)** with buttons for player interaction.
- **Randomized color sequences** that increase in length as levels progress.
- **Visual feedback** when the player selects the correct or incorrect color.
- **Signals and slots mechanism** to handle game logic and UI updates.

## Installation & Setup
### Prerequisites
- Qt 5 or Qt 6 installed on your system.
- C++ compiler (MSVC, GCC, or Clang).
- Qt Creator (recommended) or another C++ IDE.

### Clone the Repository
```sh
git clone https://github.com/yourusername/simon-game.git
cd simon-game
```

### Build & Run
1. Open the project in **Qt Creator**.
2. Configure the project with the correct Qt version.
3. Click **Build** → **Run** to start the game.

Alternatively, if using CMake:
```sh
mkdir build
cd build
cmake ..
make
./SimonGame
```

## How to Play
1. Click the **Start** button to begin the game.
2. Watch the sequence of flashing colors carefully.
3. Repeat the sequence by clicking the corresponding color buttons.
4. If correct, the sequence gets longer. If incorrect, the game restarts.

## Code Structure
```
SimonGame/
│── src/
│   ├── main.cpp          # Entry point
│   ├── mainwindow.h/cpp  # Main GUI logic
│   ├── gamemodel.h/cpp   # Game logic (sequence, checking, randomization)
│── ui/
│   ├── mainwindow.ui     # Qt Designer UI file
│── README.md             # Project documentation
│── CMakeLists.txt        # CMake build configuration (if applicable)
```

## Important Classes
- **GameModel**: Handles game logic, including generating random sequences and checking user input.
- **MainWindow**: Manages the user interface and connects signals/slots for interaction.

## Dependencies
- Qt Widgets (for UI components and event handling)
- QObject (for signal-slot mechanism)

## Future Enhancements
- Add sound effects for each color press.
- Implement different difficulty levels.
- Save and display high scores.

## License
This project is licensed under the **MIT License**.

## Author
Created by Phuc Hoang and Chanphone Visathip

Feel free to contribute or report issues!

