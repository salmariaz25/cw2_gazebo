Salma Riaz 
M00982503
PDE4430
CW 2 
Readme – Report
Github link : https://github.com/salmariaz25/cw2_gazebo.git

The objective of this assignment was to design and implement a robot which is capable of navigating through a Gazebo simulation environment, which includes obstacles represented by cylinders and three different-sized spheres. 
The task was to carry these spheres to a designated goal post. 
The assignment involved the use of Gazebo for simulation, Xacro for URDF generation, and ROS for robot control.
To ensure version control, the robot's codebase was regularly committed to the Git repository (provided above) throughout the development process.

How to run the program:
1.	roslaunch my_robot_urdf world.launch 
this spawns the robot onto the provided assessment_world

2.	roslaunch assessment_world objects.launch
this launchs the spheres to the world

3.	rosrun teleop_twist_keyboard teleop_twist_keyboard.py
to make the robot move using the keyboard

Robot design:
The designed robot is a cylindrical shaped body with a camera, lidar, a head, two arms, two wheels on its side, and two caster wheels beneath for easy movement.
To enable the robot to carry the spheres to the goal, two arms were incorporated into the robot's URDF on its sides. These arms provides a stable platform for the spheres, ensuring that they stay within the robot's area during transportation.
Although I was not able to program the autonomous navigation for the robot to detects the spheres and move on its own to complete the task, I had still equipped it with a camera and a Hokuyo laser scanner lidar to avoid collision with the cylindrical walls as well as for autonomous path planning by using information from the camera and lidar scanner to improve its perceptual abilities for autonomous navigation. 
