# Ping-Pong Game using c++
<h2>Introduction:</h2>
	1. Built a Ping Pong game using SDL2, SDL2_image and SDL_ttf. This Project uses the SDL library to create Window,Render objects,Textures and Fonts onto the window.<br>
	2. This project was built from the scratch and had taken help of lazyfoo.net and Udacity instructors.<br>
	3. The Goal of this Game is to protect the ball from the opponet's hit trajectory. To win you have to score 5 points .


# Expected Behaviour
![Alt Text](Demo.gif)
# Dependencies For Running Locally
- cmake >= 3.7
	- All OSes: [click here for installation instructions](https://cmake.org/install/)
- make >= 4.1 (Linux, Mac), 3.81 (Windows)
	- Linux: make is installed by default on most Linux distros
	- Mac: [install Xcode command line tools to get make](https://developer.apple.com/xcode/features/)
	- Windows: [Click here for installation instructions](http://gnuwin32.sourceforge.net/packages/make.htm)
- SDL2 >= 2.0
	- All installation instructions can be found [here](https://wiki.libsdl.org/Installation)
	- Note that for Linux, an apt or apt-get installation is preferred to building from source.
- SDL_Image >= 2.0
	- All installation instructions can be found [here](https://lazyfoo.net/tutorials/SDL/06_extension_libraries_and_loading_other_image_formats/index.php). Download link can be found [here](https://www.libsdl.org/tmp/SDL_image/) is the official site.
- SDL_ttf >= 2.0
	- Follow the same installation procedure as SDL_Image. Download link to library is [here](https://www.libsdl.org/projects/SDL_ttf/).
	- gcc/g++ >= 5.4
	- Linux: gcc / g++ is installed by default on most Linux distros
	- Mac: same deal as make - [install Xcode command line tools](https://developer.apple.com/xcode/features/)
	- Windows: recommend using [MinGW](http://www.mingw.org/)
# Game Play Controls
- Left Player Moves Up and Down with W/S Buttons
- Right Player Moves Up and Down with Up arrow and Down arrow key respectively
- Space to Start , Pause and Continue the Game
# Class Structure (Class Diagram And Explaination)
![Alt Text](class.png)
# Build Instructions
- Make sure your project is in Current Working Directory ,  Image and Font Problems occur if not set. Please verify it.
- Make a Build Directory mkdir build
- Goto Build cd build
- Follow Commands : cmake .. && make
- ./PingPong
# Points Addressed 

- The project demonstrates an understanding of C++ functions and control structures.
	Across all the classes functions and control statements were used.

- A variety of control structures are used in the project.
	- In player.cpp line 33 switch control statement is used
	- In many classes including Player.cpp if-else and if statements were used

- The project accepts user input and processes the input.
	- In Game.cpp in line 124,147,148 program takes user input and processes it to render the position of the dasher.
- The project uses smart pointers instead of raw pointers.
	- In Game.h from line 26- 28 used shared pointers to implement the Ball , Left_player and Right_player objects
- The project uses Object Oriented Programming techniques.
	- compositon relation ship in Game.h
	- Inheritance single parent to child relation ship between Player.h and Left_player,Right_player.
- Classes use appropriate access specifiers for class members.
	- All clasess have respective public and private and inheritance from public.
- Note : No MultiThreading was used. As it was not needed for the small game.
