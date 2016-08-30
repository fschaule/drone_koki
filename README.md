## Koki

The project uses the libkoki marker to control the AR.Drone 2.0. If there is a libkoki marker with the id = 0 in the field of view of the camera of the drone the drone tries to follow it. Thereby it tries to keep a certain distance to the marker.

# Requirements

To run this project the following libraries are required:

* OpenCV with Python bindings
* Pygame
* PS-Drone http://www.playsheep.de/drone/downloads.html
* libkoki https://github.com/chrisjameskirkham/libkoki
* python bindings for libkoki git://srobo.org/pykoki.git

# Usage

The code allows a manual override of the Drone control at any time. Even if the drone is in the automous flight the manuel comands work but maybe overwritten if the marker is in the field of view. The focus must be on the black pygame window not on the video window. Steering:

Key | Action
----- | ------
W/A/S/D | forward, backward, left, right
Q/E | turn right / left
UP/DOWN | arrow keys fly upwards / downwards
ENTER | takeoff
SPACE | land
BACKSPACE | emergency rotor stop (drop like a stone)
1 | activate autonmous flight mode
2 | deactive autonmous flight mode




