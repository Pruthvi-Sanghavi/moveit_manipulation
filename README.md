# PickItUp
Repository for project 4 of Path Planning.

## Authors
- Pruthvi Sanghavi
- Achal Vyas

## Baxter package installation
Open the terminal and type,
```
sudo apt-get install gazebo7 ros-kinetic-qt-build ros-kinetic-gazebo-ros-control ros-kinetic-gazebo-ros-pkgs ros-kinetic-ros-control ros-kinetic-control-toolbox ros-kinetic-realtime-tools ros-kinetic-ros-controllers ros-kinetic-xacro python-wstool ros-kinetic-tf-conversions ros-kinetic-kdl-parser

cd ~/<workspace>/src
wstool init .
wstool merge https://raw.githubusercontent.com/RethinkRobotics/baxter_simulator/kinetic-devel/baxter_simulator.rosinstall
wstool update
source /opt/ros/kinetic/setup.bash
cd ~/<workspace>
catkin_make
```

## Run Instructions
Open a terminal and type
```
cd <workspace>/src
git clone https://github.com/Pruthvi-Sanghavi/PickItUp.git
cd ..
source devel/setup.bash
./src/baxter/baxter.sh sim
roslaunch baxter_gazebo baxter_world.launch
```
In another terminal,
```
cd <workspace>
source devel/setup.bash
rosrun pickItUp ik_pick_and_place_demo.py
```
### Results
![result](https://github.com/Pruthvi-Sanghavi/PickItUp/blob/master/proj4.gif)
