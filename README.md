# drok3 description

#### 설치
	cd catkin_ws/src

	git clone https://github.com/ola31/drok3_description.git

	git clone https://github.com/ola31/cmdvel_to_cmdvel2.git

	git clone https://github.com/ros-perception/laser_filters.git

	cd ~/catkin_ws

	catkin build drok3_description2 cmdvel_to_cmdvel2 laser_filters

##### slam gmapping 패키지 없을 경우 
	sudo apt-get install ros-melodic-gmapping
ROS 버전에 따라서 melodic 대신 kinetic, noetic 등을 넣어서 설치

#### 실행

	roslaunch drok3_description2 gazebo.launch 

#### slam gmapping

	roslaunch drok3_description2 gazebo.launch

	roslaunch drok3_description2 display.launch

	rosrun gmapping slam_gmapping scan:=scan

#### gazebo map 경로 설정 

	gedit ~/.bashrc

  ㄴ export GAZEBO_MODEL_PATH=~/catkin_ws/src/drok3_description/world  (추가) 

  ㄴ 저장

	source ~/.bashrc
