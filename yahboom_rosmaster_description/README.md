# yahboom_rosmaster_description

`yahboom_rosmaster_description` is the ROS 2 package that contains the robot description assets for the Yahboom ROSMaster series.

## Purpose

This package stores the robot model, visualization configuration, and related assets used by the ROSMaster robot stack.

## Contents

- `urdf/` and `xacro/` robot description files.
- `meshes/` for the physical robot geometry.
- `launch/` files for visualization and robot setup.
- `rviz/` configs for RViz robot display.
- `config/` and package metadata.

## Build

From the workspace root:

```bash
cd ~/ros2_ws
source /opt/ros/<your_ros2_distro>/setup.bash
colcon build --packages-select yahboom_rosmaster_description
```

## License

BSD-3-Clause

---

Author: Alessandro Tiozzo
Date: 2026-06-25
