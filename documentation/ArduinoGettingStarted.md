# Getting Started

# Kernel Message Welcoming Arduino 101

Arduino 101 board connected to a Linux host with USB Cable

```sh
user@workstation:~$ dmesg
[82455.310461] usb 1-6: new full-speed USB device number 79 using xhci_hcd
[82455.440584] usb 1-6: New USB device found, idVendor=8087, idProduct=0ab6
[82455.440587] usb 1-6: New USB device strings: Mfr=1, Product=2, SerialNumber=3
[82455.440589] usb 1-6: Product: ARDUINO 101
[82455.440590] usb 1-6: Manufacturer: Intel
[82455.440591] usb 1-6: SerialNumber: AE6642SQ60400F1
[82455.441956] cdc_acm 1-6:1.0: ttyACM0: USB ACM device
user@workstation:~$ 
```

```sh
pymelab@workstation:~/Descargas/arduino-1.6.12$ ./arduinols -l /dev/ttyACM* ^C
pymelab@workstation:~/Descargas/arduino-1.6.12$ ls -l /dev/ttyACM* 
crw-rw---- 1 root dialout 166, 0 oct 23 12:04 /dev/ttyACM0
pymelab@workstation:~/Descargas/arduino-1.6.12$ sudo usermod -a -G dialout pymelab
```

## Arduino 101 Sketch Verification

```sh
    Sketch uses 29,473 bytes (14%) of program storage space. Maximum is 196,608 bytes.
```

## Arduino 101 Sketch Upload

```sh
Sketch uses 29,529 bytes (15%) of program storage space. Maximum is 196,608 bytes.
starting download script
Args to shell: /home/xe1gyq/.arduino15/packages/Intel/tools/sketchUploader/1.6.4+1.14/x86/bin /tmp/buildb7caae573e48d28ad6fc59334ba5d217.tmp/sketch_mar19a.ino.elf /dev/ttyACM1 quiet
Serial Port PORT
BIN FILE /tmp/buildb7caae573e48d28ad6fc59334ba5d217.tmp/sketch_mar19a.ino.bin
wating for Arduino 101 device... 
Using dfu-util to send  /tmp/buildb7caae573e48d28ad6fc59334ba5d217.tmp/sketch_mar19a.ino.bin
dfu-util 0.8

Copyright 2005-2009 Weston Schmidt, Harald Welte and OpenMoko Inc.
Copyright 2010-2014 Tormod Volden and Stefan Schmidt
This program is Free Software and has ABSOLUTELY NO WARRANTY
Please report bugs to dfu-util@lists.gnumonks.org

dfu-util: Invalid DFU suffix signature
dfu-util: A valid DFU suffix will be required in a future dfu-util release!!!
Opening DFU capable USB device...
ID 8087:0aba
Run-time device DFU version 0011
Claiming USB DFU Interface...
Setting Alternate Setting #7 ...
Determining device status: state = dfuIDLE, status = 0
dfuIDLE, continuing
DFU mode device DFU version 0011
Device returned transfer size 2048
Copying data from PC to DFU device

Download	[                         ]   0%            0 bytes
Download	[==                       ]  10%         2048 bytes
Download	[=====                    ]  21%         4096 bytes
Download	[========                 ]  32%         6144 bytes
Download	[==========               ]  43%         8192 bytes
Download	[=============            ]  54%        10240 bytes
Download	[================         ]  65%        12288 bytes
Download	[===================      ]  76%        14336 bytesdfu-util: can't detach

Download	[=====================    ]  87%        16384 bytes
Download	[======================== ]  98%        16724 bytes
Download	[=========================] 100%        16724 bytes
Download done.
Sent a total of 16724 bytes
state(2) = dfuIDLE, status(0) = No error condition is present
Done!
Resetting USB to switch back to runtime mode
Sketch will execute in about 5 seconds.
```

## Examples

- [CurieIMU Orientation Visualiser](https://www.arduino.cc/en/Tutorial/Genuino101CurieIMUOrientationVisualiser)
- [CurieIMU Step Counter](https://www.arduino.cc/en/Tutorial/Genuino101CurieIMUStepCounter)
- [CurieBLE Heart Rate Monitor](https://www.arduino.cc/en/Tutorial/Genuino101CurieBLEHeartRateMonitor)
