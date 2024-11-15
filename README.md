freebuoyancy_gazebo
===================

A Gazebo plugin to simulate underwater vehicles.

<p align="center">
  <img src="doc/demo_fall.gif">
</p>

## Gazebo plugin
The package builds two Gazebo plugins:

- freebuoyancy_gazebo (model plugin)
simulates buoyancy and viscous force from water


### Dependencies
Along with ROS you will need the following pkgs, for example I am using ROS2 humble:

```bash
sudo apt install ros-humble-urdf ros-humble-urdfdom ros-humble-urdfdom-headers
sudo apt install liburdfdom-dev liburdfdom-headers-dev

```




### Install
After cloning
```bash
cd freebuoyancy_gazebo
mkdir build
cd build
cmake ..
make
sudo make install
```
