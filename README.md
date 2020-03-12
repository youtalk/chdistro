# chdistro

`chdistro`: Change the `ROS_DISTRO` and working space with a single command.

## Install

```sh
$ pushd ~/.local/bin && wget https://raw.githubusercontent.com/youtalk/chdistro/master$SHELL/chdistro && chmod 755 chdistro && popd
```

## Usage

```sh
$ chdistro --help
chdistro ROS_DISTRO [WORKSPACE_DIR]
```

### ROS 2

```sh
$ chdistro dashing
ROS_DISTRO=dashing
ROS_PYTHON_VERSION=3
ROS_VERSION=2
ROS_HOME=/home/$USER/.ros
ROS_LOCALHOST_ONLY=1
```

```sh
$ chdistro dashing ~/ros/dashing
ROS_DISTRO=dashing
ROS_PYTHON_VERSION=3
ROS_VERSION=2
ROS_HOME=/home/$USER/.ros
ROS_LOCALHOST_ONLY=1
ROS_WORKSPACE=/home/$USER/ros/dashing
```

### ROS 1

```sh
$ chdistro melodic
ROS_HOME=/home/$USER/.ros
ROS_WORKSPACE=/home/$USER/ros/melodic
ROS_DISTRO=melodic
ROS_ETC_DIR=/opt/ros/melodic/etc/ros
ROS_PACKAGE_PATH=/opt/ros/melodic/share
ROS_PYTHON_VERSION=2
ROS_VERSION=1
ROS_ROOT=/opt/ros/melodic/share/ros
ROS_MASTER_URI=http://localhost:11311
ROSLISP_PACKAGE_DIRECTORIES=
```

```sh
$ chdistro melodic ~/ros/melodic
ROS_DISTRO=melodic
ROS_ETC_DIR=/opt/ros/melodic/etc/ros
ROS_PACKAGE_PATH=/opt/ros/melodic/share
ROS_PYTHON_VERSION=2
ROS_VERSION=1
ROS_ROOT=/opt/ros/melodic/share/ros
ROS_MASTER_URI=http://localhost:11311
ROSLISP_PACKAGE_DIRECTORIES=
ROS_HOME=/home/$USER/.ros
ROS_WORKSPACE=/home/$USER/ros/melodic
```
