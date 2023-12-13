
# Differential Drive Robot [PK-BOT]

A simple Differential Drive Robot simulated in gazebo.
(Tested on ROS2 Foxy Only)




## Deployment

Install the following dependencies before running the project

```bash
  pip install xacro
  sudo apt install ros-foxy-gazebo-ros-pkgs
```

To deploy this project run

```bash
  mkdir -p colcon_ws/src
  cd colcon_ws/src
  git clone https://github.com/a-hamzah/diff_bot.git
  cd ..
  colcon build
```

Launch gazebo simulation

```bash
  ros2 launch diff_bot launch_sim.launch.py
  OR
  ros2 launch diff_bot nust_world.launch.py
```

Run teleop twist keyboard node in a new terminal+

```bash
  ros2 run teleop_twist_keyboard teleop_twist_keyboard
```

For rviz, open a new terminal and type

```bash
  rviz2
```
In RVIZ, Click on add and select Robot Model, Change its topic to robot_description

## Screenshots

![Screenshot from 2023-12-01 22-01-45](https://github.com/a-hamzah/diff_bot/assets/25130682/13536e3a-82b3-4dde-9bb0-2494d180ec17)

## Future Work

- Add rviz in launch file
