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
  
> git clone github.com/ihom3/homeassistnat-ws281x-rpi-gpio
