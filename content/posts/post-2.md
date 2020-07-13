---
title: "MediaBox"
date: 2020-07-13
description: "How I made a local network media streaming system using Raspberry Pi 3"
tags: [Raspberry Pi]
---
### Step 1: Download the Raspberry Pi OS to an SD hard  
[Here's](https://www.raspberrypi.org/downloads/) where you'll find it. I used a 16GB card.
### Step 2: Set up the Raspberry Pi.
![Setup](https://i.imgur.com/7eFRgL8.gifv)
You'll need:
* a USB mouse
* a USB keyboard
* a display
* a router
* an ethernet cable to attach the router with
After inserting the aforementioned devices and the SD card, connect the Pi to a power source. Install the OS (do not install LibreELEC for this project)
### Step 3: Install KODI
Go to the terminal and type the following command
`$	sudo apt get kodi`
### Step 4: Configure KODI
Once installed, 
> Open Kodi and go to settings > Go to "Service settings" then "Control" > Enable "Allow remote control via HTTP"
Make sure the "Web interface" is set to "Kodi web interface - Chorus2"
![KODI config](https://i.imgur.com/e4Qnyc8.jpg)
### Step 5: Add Media
Store the media you'd like to stream onto a storage device and attach it to the Pi.
For instance go to "Movies"> Browse the movie you'd like to add.
### Step 6: Get a static IP
Go to the terminal and type
`sudo nano /etc/dhcpcd.conf`
Follow [this](https://thepihut.com/blogs/raspberry-pi-tutorials/how-to-give-your-raspberry-pi-a-static-ip-address-update) comprehensive guide for what to do next.
### Step 7: Make the system headless
Once the router is configured, Go to terminal and type the following command:
`sudo crontab -e`
Once the file opens, add the following line to the file:
`@reboot kodi --standalone`
This step makes sure one does not need to setup the Pi each time to use KODI.

## How to Use it:
1. Attach the router to the Pi via an ethernet cable. Connect the Pi and the router to a power supply.
2. Connect your device to the router network.
3. Open a browser and type the IP address followed by ':8080'. For instance, '192.7.1.2:8080'. 
4. Browse from the media you've added to KODI previously and watch it on your device.   
