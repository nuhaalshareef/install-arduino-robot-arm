# install-arduino-robot-arm
Make sure all these commands are installed :

```
 mkdir -p ~/catkin_ws/src
 cd ~/catkin_ws/
 catkin_make
 cd ~/catkin_ws/src
```
# install source code 
```
git clone https://github.com/smart-methods/arduino_robot_arm.git
``` 
 We complete the rest of the installation commands ..
```
cd ~/catkin_ws
``` 
```
rosdep install --from-paths src --ignore-src -r -y
```
* For noetic 
```
 sudo apt-get install ros-noetic-moveit
 sudo apt-get install ros-noetic-joint-state-publisher ros-noetic-joint-state-publisher-gui
 sudo apt-get install ros-noetic-gazebo-ros-control joint-state-publisher
 sudo apt-get install ros-noetic-ros-controllers ros-noetic-ros-control
```
```
sudo nano ~/.bashrc
```
* at the end of the (bashrc) file add the follwing line .. 
```
source /home/nuha/catkin_ws/devel/setup.bash
```
Then
( ctrl+o )then enter then ( ctrl+x )
```
source ~/.bashrc
```
* open the robot arm using the command :
```
roslaunch robot_arm_pkg check_motors.launch
```
# testing
![unnamed (4)](https://user-images.githubusercontent.com/108008564/181065537-4100a1b3-0cba-45f2-ae85-2a933469b5ba.jpg)
![unnamed (3)](https://user-images.githubusercontent.com/108008564/181065621-0fbdceba-7216-4855-90b2-0a71e228d8cc.jpg)

