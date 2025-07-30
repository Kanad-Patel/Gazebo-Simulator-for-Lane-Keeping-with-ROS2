# Gazebo Simulator for Lane Keeping with ROS2

![License](https://img.shields.io/badge/license-open--source-blue.svg)

## Overview

This project is a simulator and platform designed for a lane-keeping car using **ROS2** and **Gazebo**. It was developed as part of the course **ENR 508: Mobile Robots** at Ahmedabad University. The simulator runs a lane-keeping algorithm and allows for testing and development of autonomous driving systems within a simulated environment.

The included video `output1.avi` demonstrates the lane-keeping algorithm working in the simulation.

## Features

- **Lane-Keeping Algorithm**: A core feature of the project that allows the simulated car to stay within lane boundaries.
- **ROS2 Integration**: The simulation is built on **ROS2 Humble Hawksbill**, a widely-used robotics middleware.
- **Gazebo Simulation**: Uses **Gazebo** as the simulation environment for accurate physics-based performance.

## Requirements

To run this project, you will need:
- **ROS2 Humble Hawksbill** installed on **Ubuntu 22.04** (native installation recommended over virtual machines).
- **Gazebo** simulation environment with necessary ROS2 plugins.

## Installation & Setup

### 1. Clone the Repository

Clone the repository into your ROS2 workspace:
```bash
git clone https://github.com/Kanad-Patel/Gazebo-Simulator-for-Lane-Keeping-with-ROS2.git
cd Gazebo-Simulator-for-Lane-Keeping-with-ROS2
```
### 2. Run the Simulator

Run the following command in your terminal to launch Gazebo with all necessary ROS2 plugins:

bash
```
gazebo --verbose {Path to car_pkg in your system}/src/car_pkg/worlds/naya.sdf -s libgazebo_ros_factory.so
```
This will start the simulator, and the camera output from the simulated car will publish images to the images_raw topic.

### 3. Viewing Output
Once the simulator is running, you can subscribe to the images_raw topic to view the camera feed and monitor the lane-keeping algorithm in action.

