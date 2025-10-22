🤖 Two-Link Robot (URDF Model)
📖 Overview

This project defines a simple two-link robotic arm using URDF (Unified Robot Description Format) in XML.
It demonstrates how to model robot links, joints, and their relationships for use in ROS2 simulations, such as in RViz or Gazebo.

🧩 Robot Structure
🔹 Base Link

A blue box representing the robot’s base.

Size: 0.5 x 0.5 x 0.1 meters.

🔹 Link 1

A green cylinder attached to the base via joint1.

Length: 1.0 m, Radius: 0.05 m.

Rotates around the Z-axis (revolute joint).

🔹 Link 2

A red cylinder attached to link1 via joint2.


Length: 0.8 m, Radius: 0.04 m.

Rotates around the Y-axis (revolute joint).

⚙️ Joints

| Joint Name | Type     | Parent Link | Child Link | Axis  | Rotation Limit (radians) | Effort | Velocity |
| ---------- | -------- | ----------- | ---------- | ----- | ------------------------ | ------ | -------- |
| joint1     | Revolute | base_link   | link1      | 0 0 1 | -1.57 → +1.57            | 5      | 2        |
| joint2     | Revolute | link1       | link2      | 0 1 0 | -1.57 → +1.57            | 3      | 2        |

🧠 Concepts Demonstrated

Basic URDF robot modeling

Link and joint hierarchy

Visual geometry and colors

Revolute joint configuration

Axis, limits, and origin definitions
