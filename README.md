
Instructions for Programming Arduino with USBasp device.

When my Arduino can no longer be programmed with the serial USB port, I use the ICSP pins to reload the bootloader. I've found the single most reliable way to program the Arduino is witha USBASP programmer. You can find them on ebay for just a few bucks. I suggest getting one with 3.3/5V selectable voltage, as well as a 10 pin to 6 pin adapter. (the USBASP typically has 10 pins, Arduino has 6).

I'm using one like this: http://www.fischl.de/usbasp/ (as the web is not reliable, I saved a PDF in the doc folder here)

Unfortunately the devices are not plug & play; drivers need to be installed manually.

Download and run Zadig from http://zadig.akeo.ie/  (it does not need to be installed, just run the executable)

It should find your device (if not, select from dropdown). Simply install the software:

![alt text](https://github.com/gojimmypi/Arduino-USPasp/blob/master/images/Zadig.png "Zadig screen")

You should then find it in Device Manager under "Universal Serial Bus Devices"

![alt text](https://github.com/gojimmypi/Arduino-USPasp/blob/master/images/DeviceManagerItem.png "Devicer Manager Item") 

Once you have confirmed your system recognizes the USBasp, select it sd the programmer in the Arduino IDE:

![alt text](https://github.com/gojimmypi/Arduino-USPasp/blob/master/images/ArduinoSelect-USBasp.png "Arduino Select USPasp")

When connecting the cable, be sure to pay attention to the pin orientation. The ribbon cable will typically have a red indicator for pin one. On the Arduino, there's typically a little white dot near pin 1.

![alt text](https://github.com/gojimmypi/Arduino-USPasp/blob/master/images/ArduinoICSP-Pin1.png "Arduino ICSP Pin 1")

After connecting the USBasp to the Arduino, flash a new bootloader onto it:

![alt text](https://github.com/gojimmypi/Arduino-USPasp/blob/master/images/ArduinoBurnBootloader.PNG "boot loader")


