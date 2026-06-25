# yahboom_rosmaster

A ROS 2 repository for the Yahboom ROSMaster robot series.

## Overview

This repository contains the ROS 2 package stack for the Yahboom ROSMaster robot.
The root workspace is a metapackage wrapper around the robot description package.

## Package layout

- `yahboom_rosmaster/`
  - `yahboom_rosmaster/` — ROS 2 metapackage
  - `yahboom_rosmaster_description/` — robot description assets and URDF/XACRO model files

## Included packages

- `yahboom_rosmaster`
  - A minimal `ament_cmake` metapackage.
  - Depends on `yahboom_rosmaster_description`.
- `yahboom_rosmaster_description`
  - Contains robot meshes, URDF/XACRO files, launch descriptions, and RViz configs.

## Requirements

- ROS 2 distribution with `ament_cmake` (for example: Humble, Iron, or later)
- `colcon` build tools
- Linux-based ROS 2 environment

## Build instructions

From the workspace root:

```bash
cd ~/ros2_ws/src/yahboom_rosmaster
source /opt/ros/<your_ros2_distro>/setup.bash
colcon build --packages-select yahboom_rosmaster yahboom_rosmaster_description
source install/setup.bash
```

If the workspace root is `~/ros2_ws`, use:

```bash
cd ~/ros2_ws
source /opt/ros/<your_ros2_distro>/setup.bash
colcon build --packages-select yahboom_rosmaster yahboom_rosmaster_description
source install/setup.bash
```

## License

BSD-3-Clause

---

Author: Alessandro Tiozzo
Date: 2026-06-25
