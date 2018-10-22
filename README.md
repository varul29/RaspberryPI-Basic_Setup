# Raspberry Pi 3 Model B

### Installation and Image Configuration

- Install OS Raspbian [imagefile](https://www.raspberrypi.org/downloads/)
- Make the bootable SD card containing using software "Win32 Disk Imager" or "Power ISO"
- Insert Bootable SD card in Raspberry Pi SD slot

Give power to Raspberry pi through micro USB port and connect keybopard, mouse, HDMI port of Diplay Screen with

***Enable the VNC settings so that it will be easily connected to VNC viewer in Laptop or Desktop*** 

### For Connecting the Raspberry pi via Laptop using LAN Port
  
  - Power Up the RPI through micro USB port
  - Connect the LAN port with Laptop
  - open cmd prompt
  - Write "ipconfig"
  - In Ethernet Adapter option it will show Raspberry PI the default local IP (copy and save it in notepad)
  - Install VNCviewer
  - After installation, Open VNC viewer -> File -> New Connection
  - Type the default Ip copied before, Give Friendly name to raspberry pi(If user want)
  - Write the default Username = "pi" and Password = "raspberry" (if no user id password changed by the user)
  
  ### You will able to see the Raspbian OS system
  
  - Open CLI of Raspbian
  - Write the commands
       - sudo apt-upgrade
       - sudo apt-update
     
  ### For Python
        Download and install smbus library on Raspberry pi. Steps to install smbus are provided at:

        https://pypi.python.org/pypi/smbus-cffi/0.5.1
        
  ### For Java
        
        Download and install pi4j library on Raspberry pi. Steps to install pi4j are provided at:

        http://pi4j.com/install.html
  
  
  
