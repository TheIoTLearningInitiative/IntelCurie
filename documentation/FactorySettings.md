# Factory Settings

> Use the Flashpack utility to restore the factory settings and the original bootloader of the Arduino 101. Please consult the README and follow the instructions for your environment.  [Flashpack](https://downloadcenter.intel.com/downloads/eula/25470/Arduino-101-software-package?httpDown=https%3A%2F%2Fdownloadmirror.intel.com%2F25470%2Feng%2Farduino101-factory_recovery-flashpack.tar.bz2)

```sh
user@workstation:~/Download$ tar xvf arduino101-factory_recovery-flashpack.tar.bz2 
arduino101-factory_recovery-flashpack/
arduino101-factory_recovery-flashpack/bin/
arduino101-factory_recovery-flashpack/bin_osx/
arduino101-factory_recovery-flashpack/create_flasher.sh
arduino101-factory_recovery-flashpack/DFU-UTIL.readme
arduino101-factory_recovery-flashpack/drivers/
arduino101-factory_recovery-flashpack/flash_dfu.bat
arduino101-factory_recovery-flashpack/flash_dfu.sh
arduino101-factory_recovery-flashpack/flash_jtag.bat
arduino101-factory_recovery-flashpack/flash_jtag.sh
arduino101-factory_recovery-flashpack/fwversion.bat
arduino101-factory_recovery-flashpack/fwversion.sh
arduino101-factory_recovery-flashpack/images/
arduino101-factory_recovery-flashpack/images.dist/
arduino101-factory_recovery-flashpack/OSX-FTDI-Fix.sh
arduino101-factory_recovery-flashpack/README.md
arduino101-factory_recovery-flashpack/README.pdf
arduino101-factory_recovery-flashpack/scripts/
arduino101-factory_recovery-flashpack/utilities/
arduino101-factory_recovery-flashpack/utilities/fwversion/
arduino101-factory_recovery-flashpack/utilities/fwversion/readbin.c
arduino101-factory_recovery-flashpack/utilities/fwversion/README
arduino101-factory_recovery-flashpack/scripts/board/
arduino101-factory_recovery-flashpack/scripts/flash-jtag.cfg
arduino101-factory_recovery-flashpack/scripts/interface/
arduino101-factory_recovery-flashpack/scripts/target/
arduino101-factory_recovery-flashpack/scripts/target/quark_x10xx.cfg
arduino101-factory_recovery-flashpack/scripts/interface/ftdi/
arduino101-factory_recovery-flashpack/scripts/interface/ftdi/atpdev.cfg
arduino101-factory_recovery-flashpack/scripts/interface/ftdi/flyswatter2.cfg
arduino101-factory_recovery-flashpack/scripts/interface/ftdi/olimex-arm-usb-ocd-h.cfg
arduino101-factory_recovery-flashpack/scripts/board/quark_se-arc.cfg
arduino101-factory_recovery-flashpack/scripts/board/quark_se-cltap.cfg
arduino101-factory_recovery-flashpack/scripts/board/quark_se-lmt.cfg
arduino101-factory_recovery-flashpack/scripts/board/quark_se.cfg
arduino101-factory_recovery-flashpack/scripts/board/quark_x10xx_board.cfg
arduino101-factory_recovery-flashpack/images.dist/firmware/
arduino101-factory_recovery-flashpack/images.dist/firmware/ble_core/
arduino101-factory_recovery-flashpack/images.dist/firmware/partition.conf
arduino101-factory_recovery-flashpack/images.dist/firmware/ble_core/image.bin
arduino101-factory_recovery-flashpack/images/firmware/
arduino101-factory_recovery-flashpack/images/firmware/arc.bin
arduino101-factory_recovery-flashpack/images/firmware/ble_core/
arduino101-factory_recovery-flashpack/images/firmware/bootloader_quark.bin
arduino101-factory_recovery-flashpack/images/firmware/bootupdater.bin
arduino101-factory_recovery-flashpack/images/firmware/FSRom.bin
arduino101-factory_recovery-flashpack/images/firmware/partition.conf
arduino101-factory_recovery-flashpack/images/firmware/quark.0.bin
arduino101-factory_recovery-flashpack/images/firmware/quark.1.bin
arduino101-factory_recovery-flashpack/images/firmware/quark.bin
arduino101-factory_recovery-flashpack/images/firmware/quark.padded.bin
arduino101-factory_recovery-flashpack/images/firmware/ble_core/image.bin
arduino101-factory_recovery-flashpack/drivers/rules.d/
arduino101-factory_recovery-flashpack/drivers/rules.d/99-dfu.rules
arduino101-factory_recovery-flashpack/drivers/rules.d/99-openocd.rules
arduino101-factory_recovery-flashpack/bin_osx/dfu-prefix
arduino101-factory_recovery-flashpack/bin_osx/dfu-suffix
arduino101-factory_recovery-flashpack/bin_osx/dfu-util
arduino101-factory_recovery-flashpack/bin_osx/libusb-1.0.0.dylib
arduino101-factory_recovery-flashpack/bin_osx/libusb-1.0.a
arduino101-factory_recovery-flashpack/bin_osx/libusb-1.0.dylib
arduino101-factory_recovery-flashpack/bin_osx/libusb-1.0.la
arduino101-factory_recovery-flashpack/bin_osx/LICENSE
arduino101-factory_recovery-flashpack/bin_osx/LICENSE.dfu-util
arduino101-factory_recovery-flashpack/bin_osx/LICENSE.libusb
arduino101-factory_recovery-flashpack/bin_osx/openocd
arduino101-factory_recovery-flashpack/bin_osx/readbin
arduino101-factory_recovery-flashpack/bin/dfu-util
arduino101-factory_recovery-flashpack/bin/dfu-util.32
arduino101-factory_recovery-flashpack/bin/dfu-util.exe
arduino101-factory_recovery-flashpack/bin/libusb-1.0.dll
arduino101-factory_recovery-flashpack/bin/libwinpthread-1.dll
arduino101-factory_recovery-flashpack/bin/LICENSE.dfu-util
arduino101-factory_recovery-flashpack/bin/openocd.exe
arduino101-factory_recovery-flashpack/bin/openocd.l32
arduino101-factory_recovery-flashpack/bin/openocd.l64
arduino101-factory_recovery-flashpack/bin/readbin
arduino101-factory_recovery-flashpack/bin/readbin.32
arduino101-factory_recovery-flashpack/bin/readbin.exe
user@workstation:~/Downloads$ 
```

```sh
user@workstation:~/Downloads$ cd arduino101-factory_recovery-flashpack/
user@workstation:~/Downloads/arduino101-factory_recovery-flashpack$ ls
bin      create_flasher.sh  drivers        flash_dfu.sh    flash_jtag.sh  fwversion.sh  images.dist      README.md   scripts
bin_osx  DFU-UTIL.readme    flash_dfu.bat  flash_jtag.bat  fwversion.bat  images        OSX-FTDI-Fix.sh  README.pdf  utilities
user@workstation:~/Downloads/arduino101-factory_recovery-flashpack$ 
```

