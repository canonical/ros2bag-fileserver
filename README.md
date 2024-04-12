#ROS 2 bag file server

This repository is hosting the rock to build the ROS 2 bag file server.
This rock is meant to be working with the [ros2bag-fileserver-k8s-operator](https://github.com/ubuntu-robotics/ros2bag-fileserver-k8s-operator).

## How to build

Build the rock:
```
rockcraft pack
```
Add the rock to the local docker images:
```
sudo /snap/rockcraft/current/bin/skopeo --insecure-policy copy oci-archive:ros2bag-fileserver_0.1_amd64.rock docker-daemon:ros2bag-fileserver:dev
```

