# docker-ubuntu-python-opencv

The Dockerfile builds an image on Ubuntu 16.04 and installs Python2 and Python3 and OpenCV with all required libraries.

Here's the DockerHub link https://hub.docker.com/r/chennavarri/ubuntu_opencv_python/

# Running this on a Mac OSX with X11 forwarding:
Running this image on Mac OSX with X11 forwarding could be a bit tricky. Here are the steps you would need to follow
- This assumes that you have brew, XQuartz and Docker with Kitematic installed on Mac OSX
  - brew install socat
  - socat TCP-LISTEN:6000,reuseaddr,fork UNIX-CLIENT:\"$DISPLAY\" &
  - xhost +
  - Open your XQuartz and in the X11 preferences-> Security tab-> [Check both i.e. "Authenticate connections" and "Allow connections from network clients"


