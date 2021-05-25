# drok3 description

	cd catkin_ws/src

	git clone https://github.com/ola31/drok3_description.git

	git clone https://github.com/ola31/cmdvel_to_cmdvel2.git

	git clone https://github.com/ros-perception/laser_filters.git

	cd ~/catkin_ws

	catkin build drok3_description2 cmdvel_to_cmdvel2 laser_filters

	roslaunch drok3_description2 gazebo.launch 

slam

	roslaunch drok3_description2 gazebo.launch

	roslaunch drok3_description2 display.launch

	rosrun gmapping slam_gmapping scan:=scan


gedit ~/.bashrc

  ㄴ export GAZEBO_MODEL_PATH=~/catkin_ws/src/drok3_description/world  (추가) 

  ㄴ 저장

source ~/.bashrc
