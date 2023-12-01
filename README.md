
# Differential Drive Robot [PK-BOT]

A simple Differential Drive Robot simulated in gazebo.
(Tested on humble and foxy)




## Deployment

Install the following dependencies first

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
```

Run teleop twist keyboard node in a new terminal+

```bash
  ros2 run teleop_twist_keyboard teleop_twist_keyboard
```

For rviz, open a new terminal and type

```bash
  rviz2
```