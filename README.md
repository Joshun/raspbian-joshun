Raspbian Joshun RPi Image
=========================

Joshun's Raspbian Image is a minimal raspbian image, with a set of custom scripts for ease of use:

raspi-setup - a script to configure initial setup of the pi - video, localisation etc.

desktop-setup - a script that runs if the user chooses to install a desktop system, consisting of fluxbox and xorg. The script asks the user if they want to install extra packages, allowing them to choose a web browser, IDE etc. The packages have been selected for their 'lightweightness', to run well on the raspberry pi.

The image is mastered using the raspbian installer, and the custom scripts were then added. The imaging was done using GNU dd, and the 'bs' parameter was used to skip copying unused disk space from the SD Card.

Customising the image is easy - change its files, then run /etc/raspi-setup/initial-boot


Initial boot password:raspberry

Username:pi Password:raspberry


This image has been set up to use 'sudo' for authentication instead of su. After the initial raspi-setup script has written configuration, the normal root account gets locked, to discourage using it.

Image Builds:
http://dl.dropbox.com/u/24027029/Raspbian%20Builds/raspbian-joshun-130712.img.7z
