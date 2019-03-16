# Ionic Docker image

The Dockerfile is based on the next Docker image: 

https://hub.docker.com/r/beevelop/ionic

To avoid errors when debugging Android apps implemented with Ionic in Android terminals, I install the adb packages to detect Android devices in Linux, and also I force the agreement with the Android SDK licenses.

To allow your Docker container access to your Android terminal via USB, use this command:

    docker run -it --privileged -v /dev/bus/usb:/dev/bus/usb inpt333/ionic bash
    
