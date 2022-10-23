# arm4dof_gazebo

## 使い方
### gazebo起動(Terminal#1)
```
roslaunch arm4dof_gazebo arm4dof.launch
```

### 動かす(Terminal#2)
```
rostopic pub /arm_controller/command trajectory_msgs/JointTrajectory '{joint_names: ["joint1", "joint2", "joint3", "joint4", "finger_joint"], points: [{positions: [1.0, 1.5, -0.5, -0.75, 0.75], time_from_start: [1, 0]}]}' -1
```
