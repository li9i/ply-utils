# `pointcloud_to_ply`

<p align="center">
  <a href="https://build.ros2.org/job/Hsrc_uJ__pointcloud_to_ply__ubuntu_jammy__source/"><img src="https://build.ros2.org/buildStatus/icon?job=Hsrc_uJ__pointcloud_to_ply__ubuntu_jammy__source" alt="Build Status"/></a>
  <a href="../LICENSE"><img src="https://img.shields.io/badge/License-BSD_3--Clause-blue.svg" alt="License: BSD 3-Clause"/></a>
</p>

Capture a point cloud from a sensor by subscribing to the topic where it publishes messages to, and store it in `.ply` or `.obj` form on disk.

Set your specific point cloud sensor topic, save location, and other params in `config/params.yaml`. Then launch the node with

```bash
ros2 launch pointcloud_to_ply pointcloud_to_ply.launch.xml
```
