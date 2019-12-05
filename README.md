# Motion-Planning-on-CARLA

<p align="center">
  <img  src="https://github.com/paulyehtw/Motion-Planning-on-CARLA/blob/master/controller_output/Results.gif">
</p>

## Introduction
This is an assignment from [Motion Planning for Self-Driving Cars](https://www.coursera.org/learn/motion-planning-self-driving-cars) course of [Self-Driving Cars Specialization](https://www.coursera.org/specializations/self-driving-cars?) on Coursera.org.

This assignment implements Motion Planning by implementing **behaviour planner**, **collision checker**, **local planner** and **velocity planner** using Python as the programming language.

The waypoints for the track are pre-defined.

To realize this function, the open sourse simulator [CARLA](http://carla.org) is introduced.

## Prerequisites
First CARLA must be installed on your machine, the CARLA loader requires **Ubuntu 16.04 or later** to run

Please go through **CARLA-Setup-Guide-_Ubuntu_.pdf** and install CARLA and all other dependencies properly.

CARLA Simulator can be downloaded [here](https://drive.google.com/file/d/1XflJ5AtZ5YIIBmorSdhYcEjENrY1sJJN/view?usp=sharing)

## How to run it
First clone this repository and put it under **PythonClient** directory.

### 1. Load the simulator
Open a terminal and do `cd ~/opt/CarlaSimulator`.

Then do `./CarlaUE4.sh /Game/Maps/Course4 -windowed -carla-server -benchmark -quality-level=Low -fps=30
`
### 2. Run the LKA controller
Open another terminal and do `cd ~/opt/CarlaSimulator/PythonClient/Course4FinalProject`.

(optional) do `sudo apt-get install python3-tk` in case you do not have `Tkinter` module.

Run `python3 module_7.py` to execute the controller

The car will start to track the lead car and avoid obstacles, stopping in front of the stop sign.

## Simulation results
The images shown below is the result of vehicle trajectory.

The green line is the track(ground truth) and the orange line is the trajectory.

<p align="center">
  <img  src="https://github.com/paulyehtw/Motion-Planning-on-CARLA/blob/master/controller_output/trajectory.png">
</p>

