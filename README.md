# UxPlay

This project is an early stage prototype of unix AirPlay server.
Work is based on https://github.com/FD-/RPiPlay.
Tested on Ubuntu 19.10 desktop.
5G Wifi connection is the must.

Features:

1. Based on Gstreamer.
1. Video and audio are supported out of the box.
1. Gstreamer decoding is plugin agnostic. Uses accelerated decoders if availible. VAAPI is preferable.
1. Automatic screen orientation.

## Installation for ubuntu

Building:

1. sudo apt-get install cmake
2. sudo apt-get install libssl-dev libavahi-compat-libdnssd-dev libgstreamer1.0-dev libgstreamer-plugins-base1.0-dev gstreamer1.0-libav
3. sudo apt-get install gstreamer1.0-vaapi (For Intel graphics)
4. mkdir build
5. cd build
6. cmake ..
7. make

## Installation for Fedora

```sh
sudo dnf install cmake gstreamer1-vaapi gstreamer1-libav gstreamermm-devel avahi-compat-howl avahi-compat-libdns_sd

mkdir build
cd build
cmake ..
make
```
