Arduino IDE
==

## Sketch

> A sketch is the name that Arduino uses for a program. It's the unit of code that is uploaded to and run on an Arduino board. [Arduino](https://www.arduino.cc/en/Tutorial/Sketch)

## Hello Arduino 101

Arduino 101 board connected to Linux host with USB Cable

```sh
    user@host:~$ dmesg
    ...
    [47507.944036] usb 5-2: new full-speed USB device number 3 using uhci_hcd
    [47508.121051] usb 5-2: New USB device found, idVendor=8087, idProduct=0aba
    [47508.121056] usb 5-2: New USB device strings: Mfr=1, Product=2, SerialNumber=3
    [47508.121059] usb 5-2: Product: ARDUINO 101
    [47508.121062] usb 5-2: Manufacturer: Intel
    [47508.121064] usb 5-2: SerialNumber: AE6642SQ54700DQ
```

## Sketch Compilation

```sh
    Sketch uses 29,473 bytes (14%) of program storage space. Maximum is 196,608 bytes.
```

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