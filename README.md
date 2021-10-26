本仓库为ROS入门教程的代码示例，包括以下ROS软件包:

| 软件包                        |                           内容                            |
| :---------------------------- | :-------------------------------------------------------: |
| **robot_sim_demo**            |        机器人仿真程序，大部分示例会用到这个软件包         |
| **topic_demo**                |     topic通信，自定义msg，包括C++和python两个版本实现     |
| **service_demo**              |   service通信，自定义srv，分别以C++和python两种语言实现   |
| **action_demo**               |     action通信，自定义action，C++和python两种语言实现     |
| **param_demo**                |         param操作，分别以C++和python两种语言实现          |
| **msgs_demo**                 |            演示msg、srv、action文件的格式规范             |
| **tf_demo**                   |     tf相关API操作演示，tf示例包括C++和python两个版本      |
| **name_demo**                 |        演示全局命名空间和局部命名空间下参数的提取         |
| **tf_follower**               |          制作mybot机器人 实现mybot跟随xbot的功能          |
| **urdf_demo**                 |             创建机器人urdf模型，在RViz中显示              |
| **navigation_sim_demo**       |    导航演示工具包，包括AMCL, Odometry Navigation等演示    |
| **slam_sim_demo**             | 同步定位与建图演示，包括Gmapping, Karto, Hector等SLAM演示 |
| **robot_orbslam2_demo**       |                      ORB_SLAM2的演示                      |
| **ros_academy_for_beginners** |        Metapacakge示例，依赖了本仓库所有的pacakge         |


1. 安装教学包所需的依赖

```sh
$ cd ~/catkin_ros
$ rosdep install --from-paths src --ignore-src --rosdistro=kinetic -y
```

2. 编译并刷新环境

```sh
$ catkin_make
$ source ~/catkin_ws/devel/setup.bash
```

3. 建议在**本地Ubuntu 16.04**下运行仿真程序。目前Gazebo模拟器的**兼容性**是一大问题，在虚拟机或配置较低的电脑上可能无法运行。**如果你的显卡是N卡，建议安装Ubuntu下的显卡驱动**。

4. 运行Gazebo仿真程序`robot_sim_demo`前，请将Gazebo升级到7.x版本以上（**推荐7.9版本**）。

  查看Gazebo版本方法

  ```sh
$ gazebo -v   #确认7.0以上，推荐7.9
  ```


