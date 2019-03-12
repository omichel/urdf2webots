# urdf2webots [![Build Status](https://travis-ci.org/omichel/urdf2webots.svg?branch=master)](https://travis-ci.org/omichel/urdf2webots)

This tool converts URDF files to a Webots-readable format.

## Install

```
git clone https://github.com/omichel/urdf2webots.git
cd urdf2webots
pip install -r requirements.txt
```

## Usage

`python urdf2webots.py someRobot.urdf [-o outputFile] [--box-collision]`

Outputs: someRobot_textures (folder), someRobot.proto.  
Test in webots: put the outputs in protos folder within webots project folder.

## Notes
urdf file should be in same folder as python code.  
This has been tested with ur10, pr2 and motoman using webots pro 7.4.3 on Ubuntu16.04.  
The repos of urdfs are here:  
  universal robot: https://github.com/ros-industrial/universal_robot/tree/kinetic-devel/ur_description  
  pr2 robot: https://github.com/PR2/pr2_common/tree/kinetic-devel/pr2_description  
  motoman robot: https://github.com/ros-industrial/motoman/tree/kinetic-devel/motoman_sia20d_support  
