# Raspberry-PI_SHT31_Firebase
  In this project I am going to post the real time data of temperature and humidity sensor to the Firebase database.
  I am using SHT31 Sensor to communicate with raspberry pi using I2C connection adapters

## For Raspberry Pi Setup 
  Please check out here

## Devices used in project 

  - Raspberry Pi 3 Model B
  - SHT31 I2C mini module
  - Raspberry Pi I2C adapter
  - I2C cable
  
*Connect the Raspberry Pi GPIO pins with I2C adapter 
*Using I2C cable, connect SHT31 sensor with 'IN' port available on sensor

### First Step after Physical connections 

  After Physical connection between SHT31(Temperature and humidity sensor) and Raspberry Pi:
    
   - Check the LED status which shows the power Connection in I2C adapter(connected with GPIO pins of RPI3) as well as in SHT31
   - After power connection open CLI of Raspberry Pi 
   - Configure all the general commands which are mentioned in "Raspberry-PI-" folder
   - detect I2C register of sensor using comman i2cdetect -y 1
   - configure firebase using "sudo pip install python-firebase"
    
## How to use firebase after configuration in RPI3

you may also learn simple documentation - mentioned in reading section of "Raspberry-Pi-" folder

    #This code should be used with every script that you will be using to connect to the Firebase database.
    #Importing I2C, Time, Firebase library in python code.
    import smbus
    import time
    from firebase import firebase
    
    # IN LAST USE: 
    #store the Host ID(provided in firebase database) in variable where you want to send the real time sensor data.  
    firebase= firebase.FirebaseApplication('host id mentioned in databse of firebase')

    #store the readings in variable and convert it into string and using firbase.post then data will be posted to databse of firebase 
    result = firebase.post('host id mentioned', {'cTemp':str(cTemp),'ftemp':str(fTemp), 'humidity':str(humidity)})
    print(result)
   
 Download (or git pull) the code in pi. Run the program.
      $> python SHT31.py
 
 
 ##Note: This code is to post the Temeprature sensor data for only one go.  




