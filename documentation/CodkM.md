# CODK-M

```sh
pymelab@workstation:~$ mkdir -p ~/CODK && cd $_
pymelab@workstation:~/CODK$ git clone https://github.com/01org/CODK-M.git
Clonar en «CODK-M»...
remote: Counting objects: 135, done.
remote: Compressing objects: 100% (7/7), done.
remote: Total 135 (delta 2), reused 0 (delta 0), pack-reused 128
Receiving objects: 100% (135/135), 1.04 MiB | 219.00 KiB/s, done.
Resolving deltas: 100% (40/40), done.
Comprobando la conectividad… hecho.
pymelab@workstation:~/CODK$ cd CODK-M/
```

```sh
pymelab@workstation:~/CODK/CODK-M$ make clone
git clone -b master https://github.com/01org/CODK-A-ARC.git /home/pymelab/CODK/CODK-M//arc
Clonar en «/home/pymelab/CODK/CODK-M//arc»...
remote: Counting objects: 164, done.
remote: Total 164 (delta 0), reused 0 (delta 0), pack-reused 163
Receiving objects: 100% (164/164), 2.34 MiB | 366.00 KiB/s, done.
Resolving deltas: 100% (58/58), done.
Comprobando la conectividad… hecho.
git clone -b master https://github.com/01org/CODK-M-X86.git /home/pymelab/CODK/CODK-M//x86
Clonar en «/home/pymelab/CODK/CODK-M//x86»...
remote: Counting objects: 88, done.
remote: Total 88 (delta 0), reused 0 (delta 0), pack-reused 88
Unpacking objects: 100% (88/88), done.
Comprobando la conectividad… hecho.
git clone -b master https://github.com/01org/CODK-M-X86-Samples.git /home/pymelab/CODK/CODK-M//x86-samples
Clonar en «/home/pymelab/CODK/CODK-M//x86-samples»...
remote: Counting objects: 270, done.
remote: Total 270 (delta 0), reused 0 (delta 0), pack-reused 270
Receiving objects: 100% (270/270), 62.98 KiB | 28.00 KiB/s, done.
Resolving deltas: 100% (140/140), done.
Comprobando la conectividad… hecho.
cd /home/pymelab/CODK/CODK-M//x86-samples && ./create_symlinks.sh
git clone -b master https://github.com/01org/CODK-Z-Flashpack.git /home/pymelab/CODK/CODK-M//flashpack
Clonar en «/home/pymelab/CODK/CODK-M//flashpack»...
remote: Counting objects: 6543, done.
remote: Compressing objects: 100% (6/6), done.
remote: Total 6543 (delta 2), reused 0 (delta 0), pack-reused 6537
Receiving objects: 100% (6543/6543), 14.68 MiB | 750.00 KiB/s, done.
Resolving deltas: 100% (1672/1672), done.
Comprobando la conectividad… hecho.
pymelab@workstation:~/CODK/CODK-M$ 
```

```sh
pymelab@workstation:~/CODK/CODK-M$ sudo make install-dep
```

```sh
pymelab@workstation:~/CODK/CODK-M$ make setup
Setting up x86 Firmware
Downloading Zephyr
nstalling Zephyr to /home/pymelab/CODK/zephyr
Downloading Zephyr SDK
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
100  362M  100  362M    0     0   402k      0  0:15:20  0:15:20 --:--:--  554kc 
Installing Zephyr SDK to /home/pymelab/CODK/zephyr-sdk
Verifying archive integrity... All good.
Uncompressing SDK for Zephyr  100%  
Installing SDK to /home/pymelab/CODK/zephyr-sdk
Creating directory /home/pymelab/CODK/zephyr-sdk
Success
 [*] Installing x86 tools... 
 [*] Installing arm tools... 
 [*] Installing arc tools... 
 [*] Installing iamcu tools... 
 [*] Installing mips tools... 
 [*] Installing nios2 tools... 
 [*] Installing additional host tools... 
Success installing SDK. SDK is ready to be used.
Setting options in ~/.zephyrrc
Please run: source /home/pymelab/CODK/zephyr/zephyr-env.sh
Setting up ARC Firmware
make[1]: se ingresa al directorio «/home/pymelab/CODK/CODK-M/arc»
Downloading ARC Toolchain
cd /tmp; curl -OL https://downloadmirror.intel.com/25470/eng/arc-toolchain-linux64-arcem-1.0.1.tar.bz2
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
100  123M  100  123M    0     0   745k      0  0:02:49  0:02:49 --:--:-- 1008k
Unpacking ARC Toolchain
tar xf /tmp/arc-toolchain-linux64-arcem-1.0.1.tar.bz2 -C /home/pymelab/CODK/CODK-M/arc/
rm /tmp/arc-toolchain-linux64-arcem-1.0.1.tar.bz2
Downloading Arduino IDE
cd /tmp; curl -OL https://github.com/arduino/Arduino/archive/1.6.9.zip
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
...
...
   creating: /home/pymelab/CODK/CODK-M/arc/corelibs-arduino101-codk-m/variants/
   creating: /home/pymelab/CODK/CODK-M/arc/corelibs-arduino101-codk-m/variants/arduino_101/
  inflating: /home/pymelab/CODK/CODK-M/arc/corelibs-arduino101-codk-m/variants/arduino_101/libarc32drv_arduino101.a  
   creating: /home/pymelab/CODK/CODK-M/arc/corelibs-arduino101-codk-m/variants/arduino_101/linker_scripts/
  inflating: /home/pymelab/CODK/CODK-M/arc/corelibs-arduino101-codk-m/variants/arduino_101/linker_scripts/flash.ld  
  inflating: /home/pymelab/CODK/CODK-M/arc/corelibs-arduino101-codk-m/variants/arduino_101/pins_arduino.h  
  inflating: /home/pymelab/CODK/CODK-M/arc/corelibs-arduino101-codk-m/variants/arduino_101/variant.cpp  
  inflating: /home/pymelab/CODK/CODK-M/arc/corelibs-arduino101-codk-m/variants/arduino_101/variant.h  
mv /home/pymelab/CODK/CODK-M/arc//corelibs-* /home/pymelab/CODK/CODK-M/arc//corelibs
rm /tmp/codk-m.zip
make[1]: se sale del directorio «/home/pymelab/CODK/CODK-M/arc»
pymelab@workstation:~/CODK/CODK-M$ 
```

```sh
pymelab@workstation:~/CODK/CODK-M$ export CODK_DIR=$(pwd)
pymelab@workstation:~/CODK/CODK-M$ source ../zephyr/zephyr-env.sh
pymelab@workstation:~/CODK/CODK-M$ 
```

```sh
pymelab@workstation:~/CODK/CODK-M$ make compile
```