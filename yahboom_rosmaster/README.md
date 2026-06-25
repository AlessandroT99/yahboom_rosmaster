# yahboom_rosmaster

`yahboom_rosmaster` is a ROS 2 metapackage that aggregates the Yahboom ROSMaster robot stack.

## Purpose

This package acts as a workspace-level entry point for the Yahboom ROSMaster robot series.
It does not contain runtime nodes; instead, it declares dependencies on description packages.

## Contents

- `package.xml` and `CMakeLists.txt` for an `ament_cmake` metapackage.
- `exec_depend` on `yahboom_rosmaster_description`.

## Build

From the workspace root:

```bash
cd ~/ros2_ws
source /opt/ros/<your_ros2_distro>/setup.bash
colcon build --packages-select yahboom_rosmaster
```

To build both packages together:

```bash
colcon build --packages-select yahboom_rosmaster yahboom_rosmaster_description
```

## License

BSD-3-Clause

---

Author: Alessandro Tiozzo
Date: 2026-06-25