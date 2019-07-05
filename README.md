# ROS_Learning
Learn how to use ROS :) It's never too old to learn.


roscd
cd ..
pwd


cd src

catkin_create_pkg my_package rospy
catkin_create_pkg <package_name> <package_dependecies>

rospack list
rospack list | grep my_package
roscd my_package 


roscd my_package
mkdir launch


touch launch/my_package_launch_file.launch

<launch>
    <!-- My Package launch file -->
    <node pkg="my_package" type="simple.py" name="ObiWan"  output="screen">
    </node>
</launch>




roslaunch my_package my_package_launch_file.launch

rospack profile

ls -la

chmod +x name_of_file.py


roscd; cd ..
catkin_make

catkin_make --only-pkg-with-deps <package_name>

catkin_make --only-pkg-with-deps my_package



