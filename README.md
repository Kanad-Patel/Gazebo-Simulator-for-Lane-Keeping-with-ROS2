# Gazebo-Simulator-for-Lane-Keeping-with-ROS2
## We are making a simulator and a platform of a lane-keeping car with ROS2 on Gazebo.
This is the project for our course ENR 508 : Mobile Robots at Ahmedabad University. Outout1.avi shows the output generated for testing our lane keeping algorithms on a video of the simulator.

## How to run the Simulator?
For running the Simulator,you will need ROS2 Humble Hawksbill and Ubuntu 22.04 installed in your system.
__Note__ : It is good to use the native Ubuntu system rather than on a virtual machine.

First clone this package in your ROS workspace using git clone and cd into it.

Once you are inside the directory run the following command in your terminal to open Gazebo with all the necessary ROS2 plugins.

```console
$ gazebo --verbose {Path to car_pkg in your system}/src/car_pkg/worlds/naya.sdf -s libgazebo_ros_factory.so
```
Now, the Simulator should have started working and the camera output from the simulator will publish images to images_raw topic. 







