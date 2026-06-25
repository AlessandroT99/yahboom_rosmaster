# yahboom_rosmaster

A ROS 2 repository for the Yahboom ROSMaster robot series.

This workspace currently contains:

- `yahboom_rosmaster` — a metapackage that aggregates robot packages.
- `yahboom_rosmaster_description` — a placeholder description package for robot assets.

## Repository layout

- `yahboom_rosmaster/`
  - `package.xml`
  - `CMakeLists.txt`
  - `README.md`
- `yahboom_rosmaster_description/`
  - `package.xml`
  - `CMakeLists.txt`
  - `README.md`

## Requirements

- ROS 2 distribution with `ament_cmake` (for example: Humble, Iron, or later)
- `colcon` build tools

## Build instructions

```bash
cd ~/ros2_ws
source /opt/ros/<your_ros2_distro>/setup.bash
colcon build --packages-select yahboom_rosmaster yahboom_rosmaster_description
source install/setup.bash
```

## License

BSD-3-Clause
