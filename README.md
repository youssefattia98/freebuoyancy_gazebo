freebuoyancy_gazebo
===================

A Gazebo plugin to simulate underwater vehicles.

<p align="center">
  <img src="doc/demo_fall.gif">
</p>

## Gazebo plugin
The package builds two Gazebo plugins:

- freebuoyancy_gazebo (world plugin)
simulates buoyancy and viscous force from water

### Install
```bash
mkdir build
cd build
make
sudo make install
```

### Test it
```bash
source gazebo.sh
gazebo --verbose worlds/underwater.world -u
```

## References

This plugin is based on the original repository of [freefloating_gazebo](https://github.com/freefloating-gazebo/freefloating_gazebo),
this is only a rework to use without ROS.