# ROS1 to ROS2 Migration

Migration of a ROS1 (Noetic) package to ROS2 (Humble), demonstrating the key differences in package structure, node API, build system, and communication patterns.

## What Changed

| Component | ROS1 | ROS2 |
|-----------|------|------|
| Build system | `catkin` | `ament_cmake` / `ament_python` |
| Node API | `rospy` / `roscpp` | `rclpy` / `rclcpp` |
| Node lifecycle | `rospy.init_node()` | `rclpy.init()` + class-based node |
| Parameters | `rospy.get_param()` | `self.declare_parameter()` |
| Launch files | `.launch` (XML) | `_launch.py` (Python) |
| Message types | `std_msgs/String` | same, but from `rclpy` imports |
| Package manifest | `package.xml` format 2 | `package.xml` format 3 |

## Stack

- ROS2 Humble (target)
- ROS1 Noetic (source)
- Python / C++

## Robotronics Club — IIT Mandi

Bonus task demonstrating ROS ecosystem migration skills.

## Author

Rohit Jangra · [github.com/Rohitjangra7370](https://github.com/Rohitjangra7370)
