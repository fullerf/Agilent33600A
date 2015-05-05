# Agilent33600A

EPICS IOC for Agilent 33600A dual channel function generator, created/managed with my [SCPI IOC Template](https://github.com/fullerf/EPICS-SCPI-Template).  Note that this IOC will NOT cover all the functionality of the Agilent 33600A function generator.  It only implements a limited parameteric control that I need for driving some transducers.  That said, it should serve as a decent starting point on other endeavors with the instrument.  I use the recently incorporated USBTMC communication protocol of the ASYN driver.  Please read the notes [here](http://www.aps.anl.gov/epics/modules/soft/asyn/R4-23/RELEASE_NOTES.html) on how to set up your ASYN driver to handle usbtmc communication.

## Current Status
* Communicates the identity of the function generator to the IOC

## Known Issues
* This is not a hot-pluggable usb device.  Plug the USB cable to the function generator and your computer, then turn the function generator on, then turn on the ioc.  If you want to swap computers, you need to power cycle the function generator and follow the previous again.
