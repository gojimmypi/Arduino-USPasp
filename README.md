
Instructions for Programming Arduino with USBasp device.

When my Arduino can no longer be programmed with the serial USB port, I use the ICSP pins to reload the bootloader. I've found the single most reliable way to program the Arduino is witha USBASP programmer. You can find them on ebay for just a few bucks. I suggest getting one with 3.3/5V selectable voltage, as well as a 10 pin to 6 pin adapter. (the USBASP typically has 10 pins, Arduino has 6).

I'm using one like this: http://www.fischl.de/usbasp/ (as the web is not reliable, I saved a PDF)

Unfortunately the devices are not plug & play & need drivers installed manually.

Download and install Zadig from http://zadig.akeo.ie/

It should find your device (if not, select from dropdown). Simply install the software.

You should then find it in Device Manager under "Universal Serial Bus Devices"







When my Arduino can no longer be programmed with the serial USB port, I use the ICSP pins to reload the bootloader. So far that's resolved problems every time for me.

I've found the single most reliable way to program the Arduino is with a USBASP programmer. You can find them on ebay for just a few bucks. I suggest getting one with 3.3/5V selectable voltage, as well as a 10 pin to 6 pin adapter. (the USBASP typically has 10 pins, Arduino has 6).

With the USBASP, you can also easily reload the bootloader (see tools - burn bootloader)

This site has great resources: [url=http://www.fischl.de/usbasp/]http://www.fischl.de/usbasp/[/url]

Note that the drivers need to be installed manually. Zadig is a great resource for this: [url=http://zadig.akeo.ie/]http://zadig.akeo.ie/[/url]