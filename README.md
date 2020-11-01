# compact-hass-arm32v7
Compact home assistant Dockerfile for arm32v7 devices.

This is the dockerfile to generate lightweight docker image of homeassistant (hass) based on Alpine Linux. The size of the resultant docker image is less than 400 Mb but fully working for generic home automation environment.

This docker image was tested on raspberry pi and chrooted Arm32v7 devices.

WEMO, Philips Hue, nmap, pushbullet, Xiaomi devices, and plex were tested.
nmap and psutil were installed for monitoring network and system resources.
** You should run docker image with --net=host option for accessing your local network resources and devices as follows:


docker run -d --net=host epitaxy/compact-hass-arm32v7
