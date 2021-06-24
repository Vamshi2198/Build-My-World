# Build-My-World

## Objective 
The goal of this project is to create a simulated world in gazebo and write a plugin to interact with it.

## Directory Structure  
```
.Build-My-World                    # Build My World Project 
├── model                          # Model files 
│   ├── Building
│   │   ├── model.config
│   │   ├── model.sdf
│   ├── Robot
│   │   ├── model.config
│   │   ├── model.sdf
├── script                         # Gazebo World plugin C++ script
│   ├── hello.cpp
├── world                          # Gazebo main World containing models 
│   ├── Myworld.world
├── CMakeLists.txt                 # Link libraries 
└──
```
## Prerequisites/Dependencies  
* Gazebo >= 7.0.
* ROS Kinetic .
* Cmake >= 4.1(mac, linux), 3.81(Windows)
* gcc/g++ >= 5.4
* Git

## Build Instructions
1. Open terminal and run `sudo apt-get update && sudo apt-get upgrade -y`
2. clone the repository with `git clone https://github.com/Vamshi2198/Build-My-World`.
3. cd into project folder and create a build folder with `mkdir build`.
4. cd into build directory `cd build`
5. Build the code with `cmake../ && make`
6. export the plugin path with `export GAZEBO_PLUGIN_PATH=${GAZEBO_PLUGIN_PATH}:(path to build directory)`.
7. cd into world directory and run `gazebo Myworld`.
