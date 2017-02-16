# 机器人仿真平台

>如果catkin_make不成功，可以尝试删除/build和/dev文件夹后重试

## 环境搭建

```shell
sudo apt install ros-kinetic-moveit
sudo apt install ros-kinetic-ros-control
sudo apt install ros-kinetic-gazebo-ros-control
sudo apt install ros-kinetic-moveit-visual-tools
```

## 基本使用

### gazebo环境

* 主要环境配置文件在pioneer3at.urdf.xacro

```shell
roslaunch zs_gazebo pioneer3at_gazebo_world.launch
```

* 机械臂模型需要添加进去

### 机械臂RViz-moveit仿真

```shell
roslaunch gamma_1500_moveit_config demo.launch
```

### 机械臂在Gazebo中的抓取grasp动作规划

* 任务进行中