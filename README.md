# Indroduction

SLAM Udacity exercise.

![Screenshot](screenshot.png)


## Startup commands

To startup the Gazebo world and the RVIS tool, run the following:
roslaunch my_robot world.launch

To startup the RTAB node run the following:
roslaunch my_robot mapping.launch

To startup the teleop node run the following:
roslaunch my_robot teleop.launch

## Debugging

Display the publishing rate of a topic.
rostopic hz /camera/rgb/image_raw /camera/depth/image_raw /camera/rgb/camera_info /scan

Check where Gazebo will load materials when launched as a ROS node
rospack plugins --attrib="gazebo_media_path" gazebo_ros

View database map creaded in .ros/rtabmap.db
rtabmap-databaseViewer ~/.ros/rtabmap.db
