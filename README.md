# Building workspace
>> cd catkin_ws
>> catkin_make

# launch two_wheel_gazebo
Launch roscore:
>> roscore

Launch gazebo. Open a new terminal:
>> cd catkin_ws
>> . devel/setup.bash
>> roslaunch mybot_gazebo mybot_world.launch

Launch rviz. Open a new terminal:
>> cd catkin_ws
>> . devel/setup.bash
>> roslaunch mybot_despcription mybot_rviz.launch

Moving the robot. Writing in the /cmd_vel topic.
Open a new terminal:
>> cd catkin_ws
>> cd .devel/setup.bash
>> rostopic pub /cmd_vel geometry_msgs/Twist "linear:
  x: 0.2
  y: 0.0
  z: 0.0
angular:
  x: 0.0
  y: 0.0
  z: 0.1"

