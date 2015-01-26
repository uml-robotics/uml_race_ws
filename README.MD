dependencies (in addition to ros hydro or indigo):

    sudo apt-get install python-wstool git-core

instructions:

make and cd into a dir to contain your race workspace

```
rosws init
rosws merge /opt/ros/$ROS_DISTRO
rosws merge https://raw.githubusercontent.com/uml-robotics/uml_race_ws/master/workspace.rosinstall
rosws up
source setup.bash
rosmake uml_race
```

create a new ros package that will contain your racecar controller
