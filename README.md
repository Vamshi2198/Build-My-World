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
* you can click [here](https://s3-us-west-1.amazonaws.com/udacity-robotics/Virtual+Machines/Lubuntu_071917/RoboVM_V2.1.0.zip) to download the virtual machine with all dependencies included. 
* you will need [7-zip](http://www.7-zip.org/download.html) to extract the image and [VMware](http://www.vmware.com/) to run the virtual machine.

## Build Instructions
1. Open terminal and run `sudo apt-get update && sudo apt-get upgrade -y`
2. clone the repository with `git clone https://github.com/Vamshi2198/Build-My-World`.
3. cd into project folder and create a build folder with `mkdir build`.
4. cd into build directory `cd build`
5. Build the code with `cmake../ && make`
6. export the plugin path with `export GAZEBO_PLUGIN_PATH=${GAZEBO_PLUGIN_PATH}:(path to build directory)`.
7. cd into world directory and run `gazebo Myworld`.

## Output 
![Gazebo Simulation showing world file](https://user-images.githubusercontent.com/85461865/123188661-691c0d00-d46a-11eb-954c-9758b737f4bd.jpg)

You will get a welcome message with my name. Inorder to change that, cd into the script directory and run `gedit hello.cpp`.
Change the name and follow the build instructions again.
