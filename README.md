# 🕹️ Classic 'Pong' Game in C - using SDL2

This project is a modern implementation of the classic **'Pong'** game, developed in C using the **SDL2 library**. The primary focus is to integrate and strengthen core programming concepts such as **modularization**, **encapsulation**, and **familiarity with SDL2** for game development.  

**The project is currently in development**, with plans to gradually add new features such as menus, sound effects, and a two-player mode.  

---

## 🛠️ Key Features  
- **Single Player vs CPU**: The game currently features a single-player mode where the player competes against a simple CPU-controlled paddle.  
- **Modularized Codebase**: The game logic is divided into separate, well-encapsulated modules for better readability and maintainability.  
- **SDL2 Integration**: SDL2 is used for rendering game objects, handling input events, and managing the game loop.  
 
---

## 🚀 Installation and Compilation  

### Requirements  
To compile and run the project, you need the following:  
- **C Compiler** (e.g., gcc)  
- **CMake** (for building the project)  
- **SDL2** and **SDL2_ttf** libraries  

On Debian/Ubuntu-based systems, install the required dependencies using:  

```bash
sudo apt update
sudo apt install gcc cmake libsdl2-dev libsdl2-ttf-dev
```

---

## 🎮 How to Play  

### Controls  
**Player (Left Paddle):**  
- `W`: Move up  
- `S`: Move down  

### Objective  
Prevent the ball from passing your side of the screen while trying to make your CPU opponent miss.  
**Each missed ball awards a point to the opposite player.**  

---

## 🔨 Development Notes  
- **CMake Build System**: A `CMakeLists.txt` file manages the build process, ensuring all necessary files are included and linked properly.  
- **Clang-Format**: A `.clang-format` configuration file is provided to maintain consistent code style.   

---

## 💡 **Planned Features**
- **Main Menu**: Add a start menu and a game over screen.
- **Sound Effects**: Introduce sound effects for paddle hits and scoring.
- **Two-Player Mode**: Allow a second player to control the right paddle using arrow keys.
- **Score Table**: Display the current score on screen during gameplay.
- **Point Accumulator**: Keep track of points for each player and display a winner when a predefined score is reached.
- **Difficulty Levels**: Allow the user to choose from different difficulty levels for the CPU opponent.

---

## 📊 **Current Status**
- **Single Player Mode**: Fully implemented. The player competes against a basic CPU-controlled paddle.
- **Game Mechanics**: Ball physics, paddle movement, and collision detection are functional.
- **Rendering**: Smooth rendering of game objects using SDL2.

