Rosnode list
Rostopic list
Rosservice list
# where you can import messages
# from std_msgs.msg import Float64
rosmsg list
Rostopic echo <topic> # print out messages on this topic

catkin_make # run this on root dir

Roslaunch
roslaunch simple_arm robot_spawn.launch
rosdep check simple_arm # check missing depth
Rosdep install -I simple_arm # to install dep

catkin_create_pkg <your_package_name> [dependency1 dependency2 …]

rqt_image_view /rgb_camera/image_raw # view camera feed


rosservice call /arm_mover/safe_move "joint_1: 1.57 joint_2: 1.57"
# set a param
rosparam set /arm_mover/max_joint_2_angle 1.57
