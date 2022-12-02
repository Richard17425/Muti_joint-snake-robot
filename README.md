# Muti_joint-snake-robot
Simulation based on ROS and Rviz
官网给出的下载链接：
[Moveit download source](https://moveit.ros.org/install/source/)

这里我在CSDN上找到一个下载的教程完成了下载：[moveit_setup](https://blog.csdn.net/qq_38156743/article/details/124131919)

关于solidworks导出urdf文件以及在rviz中的操作，在CSDN上也有一个可以参考的文章：[solidworks2urdf](https://blog.csdn.net/king845/article/details/125918110)
***
## 常见报错的解决思路

- **在编译过程中如果出现报错：**
> ERROR: cannot launch node of type [moveit_setup_assistant/moveit_setup_assistant]: Cannot locate node of type [moveit_setup_assistant] in package [moveit_setup_assistant]. Make sure file exists in package path and permission is set to executable (chmod +x)

尝试解决办法：（在主目录下）

     catkin build 
    source /opt/ros/melodic/setup.bash
    roslaunch moveit_setup_assistant setup_assistant.launch
