## rosdocked

Run ROS Indigo / Ubuntu Trusty within Docker on Ubuntu Xenial or on any platform with a shared
username, home directory, and X11.

This enables you to build and run a persistent ROS Indigo workspace as long as
you can run Docker images.

Note that any changes made outside of your home directory from within the Docker environment will not persist. If you want to add additional binary packages without having to reinstall them each time, add them to the Dockerfile and rebuild.

For more info on Docker see here: https://docs.docker.com/engine/installation/linux/ubuntulinux/

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
