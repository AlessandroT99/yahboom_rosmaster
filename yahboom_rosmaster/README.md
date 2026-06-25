# yahboom_rosmaster

`yahboom_rosmaster` is a ROS 2 metapackage that aggregates the Yahboom ROSMaster robot stack.

## What it contains

- A minimal `ament_cmake` package definition.
- A dependency on `yahboom_rosmaster_description`.

## Build

Build this package from the workspace root:

```bash
cd ~/ros2_ws
colcon build --packages-select yahboom_rosmaster
```