
# Robot Localization

In this project, you will learn to utilize ROS packages to accurately localize a mobile robot inside a provided map in the Gazebo and RViz simulation environments.

Over the course of the project, I will do the following -

- Building a mobile robot for simulated tasks.

- Creating a ROS package that launches a custom r-obot model in a Gazebo world and utilizes packages like AMCL and the Navigation Stack.

- Exploring, adding, and tuning specific parameters corresponding to each package to achieve the best possible localization results.

## Installation Instructions

The project can be complete in the provided Workspace in the Classroom. Alternatively, it can be completed on an Ubuntu System with ROS Kinetic installed on it. Some specific ROS packages might be required in order to complete the project -


``` bash
$ sudo apt-get install ros-kinetic-navigation
$ sudo apt-get install ros-kinetic-map-server
$ sudo apt-get install ros-kinetic-move-base
$ rospack profile
$ sudo apt-get install ros-kinetic-amcl
```

Once all the packages are installed, clone the repository on your system and rename the project folder to `udacity_bot`. However, it is recommended that you follow the Classroom instructions on working through the project instead of cloning the repo.


## Run the Project

After completing the project, you can launch it by running the following commands first -

```bash
$ cd ~/catkin_ws
$ catkin_make
$ source devel/setup.bash
```

And then run the following in *separate* terminals -

``` bash
$ roslaunch udacity_bot udacity_bot
$ roslaunch udacity_bot amcl
$ rosrun udacity_bot navigation goal
```
