# Build-My-World

## Objective 
The goal of this project is to create a simulated world in gazebo and write a plugin to interact with it.

##Directory Structure  
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
