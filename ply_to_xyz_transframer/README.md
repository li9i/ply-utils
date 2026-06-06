# `ply_to_xyz_transframer`

<p align="center">
  <a href="https://build.ros2.org/job/Hsrc_uJ__ply_to_xyz_transframer__ubuntu_jammy__source/"><img src="https://build.ros2.org/buildStatus/icon?job=Hsrc_uJ__ply_to_xyz_transframer__ubuntu_jammy__source" alt="Build Status"/></a>
  <a href="../LICENSE"><img src="https://img.shields.io/badge/License-BSD_3--Clause-blue.svg" alt="License: BSD 3-Clause"/></a>
</p>

Transform a `.ply` file expressed in one frame to a `.xyz` file expressed in another frame.

- step 1: Inspect `launch/ply_to_xyz_transframer.launch.xml` and set the values of args.

- step 2: Launch the node
  
  ```bash
  ros2 launch ply_to_xyz_transframer ply_to_xyz_transframer.launch.xml
  ```

- step 3 (optional): If your files are named sequentially (e.g. `Sampled_Mesh_1.ply`, `Sampled_Mesh_2.ply`, ...) then you may set `input_file_prefix` and `input_file_pattern` so that when you
  
  ```bash
  ros2 param set /ply_to_xyz_transframer input_file_id "'3'"
  ```
  
  `Sampled_Mesh_3.ply` is selected as the input `.ply` file

- step 4: Simply call the node for work
  
  ```bash
  ros2 service call /ply_to_xyz_transframer/execution/enable std_srvs/srv/Trigger
  ```
