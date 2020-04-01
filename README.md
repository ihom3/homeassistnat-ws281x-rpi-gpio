# homeassistnat-ws281x-rpi-gpio
This is a modified version of homeassistant-ws281x-control made by Github user lightning1 

**Prerequisites**
1. A working installation of homeassistant
2. A working mqtt server (mosquitto would work fine)
  > sudo apt-get install mosquitto
  
  > mosquitto -d
  
**Installation**
1. First, you are going to need to have python3 installed on the raspberry pi, if it is not already
> sudo apt-get install python3 python3-pip
2. Second, you are going to need to install the rpi_ws281x library 
> sudo apt-get install rpi_ws281x
3. Next, you are going to need to download the project. I reccomend placing it in /usr/local/src
> cd /usr/local/src
  
> git clone https://www.github.com/ihom3/homeassistnat-ws281x-rpi-gpio

4. Now, we're going to need to modify the service file (homeassistant-ws281x-rpi-gpio.service). I prefer to use nano, however you could use whatever text editor you prefer (Ex. Mousepad if you're using the desktop mode of the raspberry pi)
>sudo nano /usr/local/src/homeassistant-ws281x-rpi-gpio/homeassistant-ws281x-rpi-gpio.service
5. First, set the user field to a user that has GPIO acess rights, such as root and change the working directory/ exec start to wherever you placed the installation from step 3.

**Example**
> ...
>User=root
>Group=nogroup
>WorkingDirectory=/usr/local/src/homeassistant-ws281x-control
>ExecStart=/usr/local/src/homeassistant-ws281x-control/homeassistant-ws281x-control.py
>...
