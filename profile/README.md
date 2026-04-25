## `ros2_vendors`

This organization provides a centralized collection of vendor packages for ROS 2.

Vendor packages in ROS 2 are used to integrate and manage third-party dependencies such as external libraries, middleware components, and supporting tools that are required by ROS packages. These packages help ensure reproducible builds, consistent dependency versions, and easier cross-platform support across different ROS 2 distributions.

The goal of the `ros2-vendors` organization is to maintain and simplify access to commonly used vendor packages by providing:

- a single place for ROS 2 vendor repositories
- consistent maintenance across ROS 2 distributions
- easier dependency management for downstream projects
- support for reproducible and portable builds
- simplified integration for embedded, robotics, and industrial use cases

Examples of vendor packages include:

- `fmt_vendor`
- `bullet3_vendor`
- utility and middleware dependency wrappers

This repository contains the `ros2_vendors.repos` manifest, which can be used to import all maintained vendor packages into a workspace.

## Usage

```
mkdir ros2_ws && cd ros2_ws
mkdir src
curl -O https://raw.githubusercontent.com/ros2-vendors/ros2_vendors/jazzy/ros2_vendors.repos
vcs import src < ros2_vendors.repos
```

This allows developers to quickly bootstrap a workspace with the required vendor packages for building ROS 2 systems and related integrations.
