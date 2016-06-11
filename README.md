## rosdocked

Run ROS Ubuntu Trusty / indigo on any platform with a shared username, home
directory, and X11.

This enables you to build and run a persistent ROS Indigo workspace as long as
you can run Docker images.

### Build

This will create the image with your user/group ID and home directory.

```
./build.sh IMAGE_NAME
```

### Run

This will run the docker image.

```
./dock.sh IMAGE_NAME
```

The image shares it's  network interface with the host, so you can run this in
multiple terminals for multiple hooks into the docker environment.

### Whale

🐳
