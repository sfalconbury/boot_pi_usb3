# boot_pi_usb3


<B>Down and dirty way to boot the Raspberry Pi 4 from USB3</B>

I know there are many published ways to boot the Pi4 to USB3 on the internet. This is my way<br>

What I used for this:<br>
<B>Hardware</B><br>
•	Raspberry Pi 4 4GB Model B with 1.5GHz 64-bit quad-core ARMv8 CPU (4GB RAM)</B><br>
•	3.5A USB-C Raspberry Pi 4 Power Supply with Noise Filter<br>
•	32GB Samsung EVO+ Micro SD Card (Class 10)<br>
•	SanDisk 32G USB3 Flash Drive 
•	Micro HDMI to HDMI Cable<br>
•	USB MicroSD Card Reader<br>
<B>Software</B><br>
•	Raspbian Buster (w/desktop and software) (Kernal version 4.19)<br>
•	Etcher v1.5.63<br>
<B>Prerequisites</B><br>
•	Download and install current version of Etcher for your OS<br>
o	(https://www.balena.io/etcher/)<br>
•	Download current version of Raspbian<br>
o	(https://www.raspberrypi.org/downloads/raspbian/)<br>
•	Flash the micro SD card with the Raspbian image (use the instructions on the Etcher site)<br>
•	Flash the USB3 drive with the same Raspbian image<br>
<B>Make changes to the boot config file</B><br>
•	Mount the micro SD card<br>
•	Open the micro SD card file directory<br>
•	Find the config file and open with a text editor<br>
•	Scroll to the bottom of the file and add the following line to the config file<br>
```
program_usb_boot_mode=1
```
<B>Installing Raspbian on the Raspberry Pi</B><br>
•	Once the micro SD card and USB3 drive are ready plug them into the Raspberry Pi<br>
•	Power the Raspberry Pi<br>
•	Once the Raspberry Pi has booted to the “Welome” screen stop! There is no need to go any further or configure anything    yet.<br>
•	Shutdown the Raspberry Pi<br>
•	Remove power<br>
•	Remove the micro SD card but do not remove the USB3 drive<br>
