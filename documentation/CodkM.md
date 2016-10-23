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

```