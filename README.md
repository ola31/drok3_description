# drok3_description

cd ~/catkin_ws/src

git clone https://github.com/ola31/drok3_description.git
git clone https://github.com/ola31/cmdvel_to_cmdvel2.git

cd ~/catkin_ws
catkin build cmdvel_to_cmdvel2 drok3_description2

roslaunch drok3_description2 gazebo.launch 
