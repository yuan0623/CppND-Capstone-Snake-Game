# CPPND: Capstone Snake Game Submission

This is my submission for the Capstone project in the [Udacity C++ Nanodegree Program](https://www.udacity.com/course/c-plus-plus-nanodegree--nd213). 

In this submission, I have addressed following ruburc points:
* The project accepts user input and process the input (***see game.cpp, line 67-71***)
  * in this program, the user need to input their name to get the game started.
  * then, a welcome message is generated in the console as a step to process the input.
* The project reads data from a file andprocess the data, or the program writes data to a file (***see game.cpp, line 72-85***)
  * in this program, the user's name, score and the size of the snake will be write into record.txt file.
* The project uses move semantics to move data, instead of copying it, where possible
  * in this program I move the `Controller`, `Renderer` object into the `Game::Run()` method (see ***see main.cpp, line 17***)
* the project makes use destructor appropriately
  * in this program, I have implemented a destrctor in `game.h` and `game.cpp`, the destctor free the heap memory `_userName`
  
<img src="snake_game.gif"/>



## Dependencies for Running Locally
* cmake >= 3.7
  * All OSes: [click here for installation instructions](https://cmake.org/install/)
* make >= 4.1 (Linux, Mac), 3.81 (Windows)
  * Linux: make is installed by default on most Linux distros
  * Mac: [install Xcode command line tools to get make](https://developer.apple.com/xcode/features/)
  * Windows: [Click here for installation instructions](http://gnuwin32.sourceforge.net/packages/make.htm)
* SDL2 >= 2.0
  * All installation instructions can be found [here](https://wiki.libsdl.org/Installation)
  * Note that for Linux, an `apt` or `apt-get` installation is preferred to building from source.
* gcc/g++ >= 5.4
  * Linux: gcc / g++ is installed by default on most Linux distros
  * Mac: same deal as make - [install Xcode command line tools](https://developer.apple.com/xcode/features/)
  * Windows: recommend using [MinGW](http://www.mingw.org/)

## Basic Build Instructions

1. Clone this repo.
2. Make a build directory in the top level directory: `mkdir build && cd build`
3. Compile: `cmake .. && make`
4. Run it: `./SnakeGame`.