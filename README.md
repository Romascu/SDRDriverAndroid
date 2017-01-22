# License

This app is a fork of the free software & open-source app RTL2832U driver, Copyright (c) 2012-present Martin Marinov, under the GNU GPL v3 license. This fork (as in custom version) is under the same license.For the moment this fork it has only minimal changes,mosty administrative changes needed to enable further customization and functionality.

Link to license: https://github.com/martinmarinov/rtl_tcp_andro-

Original repository source and more info: https://github.com/martinmarinov/rtl_tcp_andro-


Further info (from the original author):

This is itself a modification of rtl_tcp and libusb-1.0 for running on Android (also works on other Linux based systems) 
 
It is compatible with the original rtl_tcp with the following exceptions: 
 
Added features: 
 - Opening devices using a file descriptor (very important for Android).
 - An additional command for closing the app remotely and setting tuner gain in percentage

 Removed features:
 - Ability to automatically open a device in JNI (without first opening it via the Android USB API)

Files modified in libusb-1.0 to create libusb-andro: 
 core.c, libusb.h and libusbi.h - to header for and implementation of the open2 function which takes an already open file descriptor 
 linux_usbfs.c - to create a libusb handle from the fd 

The modifications are released under GNU. See [COPYING](/COPYING) for details. 
 
For more information on rtl-sdr: 
http://sdr.osmocom.org/trac/wiki/rtl-sdr 
 
For more information on libusb: 
http://www.libusb.org/wiki/libusb-1.0

Based on modifications on libusb:
https://github.com/kuldeepdhaka/libusb
