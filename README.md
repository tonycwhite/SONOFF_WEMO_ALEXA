# SONOFF_WEMO_ALEXA
A replacement script for the sonoff basic device

This file has been taken mostly from 
https://github.com/kakopappa/arduino-esp8266-alexa-wemo-switch

unfortunately, i'm not a Github guru, so im not sure of the protocol for working with someone elses scripts, but that is where the credit for this program should go.

# My basic changes:

  1. the device name is now at the top of the script to make it simpler for quick changes
  2. The GPIO devices are correct for the sonoff device
  3. the information printed via serial, now displays the device mac address should you require to give it a static IP
  4. the LED is on initially, showing not connected, then flashes, and goes off to show connected (not a fan of lights in dark rooms)
  5. operation via Alexa or other home automation has the LED flash once
  6. operation of the relay is also via push switch.
  
#I'll reiterate - all credit to kakopappa!!
  
  Device - if you haven't got one yet, buy the SONOFF Basic - NOT THE RF variant - its a pain to load new firmware
  #DO NOT HAVE THE DEVICE WIRED TO MAINS WHILST TINKERING - only once put back together
  You will need a serial programming device - i use the FTDI 232.
  connect the devices as per the images, ensure the FTDI is set to 3.3v!!
  Note : the relay may not operate at 3.3v, don't despair.
    
  Usage: Ensure you have all the dependencies required - load to arduino
  
  Once the software is loaded, watch the serial screen.
  
  While looking for Wifi, the device LED will be illuminated.
  Once connected it will flash twice.
  
  Get alexa / app to scan for devices. it should apear as the name you have programmed it with.
  
  Operation of the onboard switch will toggle the relay state.
  
  
  Enjoy - £5 for a WEMO device - better than the £25 for the kosha version (in my books anyway)
  
  
