# KAM-Pi
ONVIF compatible CCTV camera based on the Raspberry Pi

Project objectives:
1) Create a CCTV camera using the Raspberry Pi board and camera ( and with sound using an inexpensive microphone )
2) Use a generic approach, to isolate from the hardware architecture (allow using a PC and a USB camera too)
3) Prefer using C++ and OOP unless practical constraints would dictate another solution, on case by case basis
4) Add an ONVIF module to allow the camera to be connected to an ONVIF compatible NVR
5) Add security features: 
        motion detection, 
        trigger alarm and SD card picture recording on blocked wiew detection, 
        alarm (via SNMP trap), 
        temperature monitoring,
        NTP client
        SD card recording when alarm triggered
        trigger alarm and SD card picture recording when connection lost
        event log
6) Create a Linux image for RaspberryPi with the KAM-Pi project included and execute it from RAM
7) Consider some exotic "nice-to-have" like face recognition, vibration detection (as the camera is attached to a surface of interest, an acceleration sensor can provide trespassing alarms), sound amplifier self adjust, etc.
8) Not the least important: provide privacy features like image authentication, live streaming authentication, speciffic firewall settings, etc.

Methods and tools:
- the main tool is Eclipse using the CDT plugin
- the project is based on the old good makefile
- where the execution time is not a constraint use the Python scripting
- as much as reasonable provide a cross-platform approach
