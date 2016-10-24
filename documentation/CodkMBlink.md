# Blink

```sh
pymelab@workstation:~/CODK/CODK-M/x86-samples$ cd Blink/
pymelab@workstation:~/CODK/CODK-M/x86-samples/Blink$ ls
Makefile  outdir  prj.conf  prj.mdef  src
pymelab@workstation:~/CODK/CODK-M/x86-samples/Blink$ 
```

```sh
pymelab@workstation:~/CODK/CODK-M/x86-samples/Blink/src$ ls -als
total 20
4 drwxrwxr-x 2 pymelab pymelab 4096 oct 23 18:55 .
4 drwxrwxr-x 4 pymelab pymelab 4096 oct 23 19:43 ..
0 lrwxrwxrwx 1 pymelab pymelab   52 oct 23 18:55 arduino -> /home/pymelab/CODK/CODK-M/x86-samples/common/arduino
4 lrwxrwxrwx 1 pymelab pymelab   64 oct 23 18:55 arduino101_services -> /home/pymelab/CODK/CODK-M/x86-samples/common/arduino101_services
4 -rw-rw-r-- 1 pymelab pymelab  922 oct 23 18:55 blink.c
4 -rw-rw-r-- 1 pymelab pymelab   65 oct 23 18:55 Makefile
pymelab@workstation:~/CODK/CODK-M/x86-samples/Blink/src$ 
```

```sh
pymelab@workstation:~/CODK/CODK-M/x86-samples/Blink$ make pristine
pymelab@workstation:~/CODK/CODK-M/x86-samples/Blink$ make
Using /home/pymelab/CODK/zephyr/boards/arduino_101/arduino_101_factory_defconfig as base
Merging /home/pymelab/CODK/zephyr/kernel/configs/micro.config
Merging prj.conf
warning: (I2C_QMSI) selects DMA_QMSI which has unmet direct dependencies (DMA && QMSI)
#
# configuration written to .config
#
make[1]: se ingresa al directorio «/home/pymelab/CODK/zephyr»
make[2]: se ingresa al directorio «/home/pymelab/CODK/CODK-M/x86-samples/Blink/outdir»
  GEN     ./Makefile
scripts/kconfig/conf --silentoldconfig Kconfig
warning: (I2C_QMSI) selects DMA_QMSI which has unmet direct dependencies (DMA && QMSI)
warning: (I2C_QMSI) selects DMA_QMSI which has unmet direct dependencies (DMA && QMSI)
make[2]: se sale del directorio «/home/pymelab/CODK/CODK-M/x86-samples/Blink/outdir»
make[2]: se ingresa al directorio «/home/pymelab/CODK/CODK-M/x86-samples/Blink/outdir»
  Using /home/pymelab/CODK/zephyr as source for kernel
  GEN     ./Makefile
  CHK     include/generated/version.h
  UPD     include/generated/version.h
  HOSTCC  scripts/gen_idt/gen_idt.o
  HOSTLD  scripts/gen_idt/gen_idt
  CHK     misc/generated/configs.c
  UPD     misc/generated/configs.c
  CHK     include/generated/offsets.h
  UPD     include/generated/offsets.h
  CHK     misc/generated/sysgen/prj.mdef
  UPD     misc/generated/sysgen/prj.mdef
  LD      lib/libc/minimal/source/stdlib/built-in.o
  CC      lib/libc/minimal/source/stdout/fprintf.o
  CC      lib/libc/minimal/source/stdout/prf.o
  CC      lib/libc/minimal/source/stdout/sprintf.o
  CC      lib/libc/minimal/source/stdout/stdout_console.o
  LD      lib/libc/minimal/source/stdout/built-in.o
  CC      lib/libc/minimal/source/string/string.o
  LD      lib/libc/minimal/source/string/built-in.o
  LD      lib/libc/minimal/source/built-in.o
  LD      lib/libc/minimal/built-in.o
  LD      lib/libc/built-in.o
  LD      lib/built-in.o
  CC      kernel/microkernel/k_task.o
  CC      kernel/microkernel/k_idle.o
  CC      kernel/microkernel/k_init.o
  CC      kernel/microkernel/k_command_packet.o
  CC      kernel/microkernel/k_move_data.o
  CC      kernel/microkernel/k_ticker.o
  CC      kernel/microkernel/k_memory_map.o
  CC      kernel/microkernel/k_memory_pool.o
  CC      kernel/microkernel/k_irq.o
  CC      kernel/microkernel/k_nop.o
  CC      kernel/microkernel/k_offload.o
  CC      kernel/microkernel/k_event.o
  CC      kernel/microkernel/k_mailbox.o
  CC      kernel/microkernel/k_mutex.o
  CC      kernel/microkernel/k_fifo.o
  CC      kernel/microkernel/k_semaphore.o
  CC      kernel/microkernel/k_timer.o
  CC      kernel/microkernel/k_pipe_buffer.o
  CC      kernel/microkernel/k_pipe.o
  CC      kernel/microkernel/k_pipe_get.o
  CC      kernel/microkernel/k_pipe_put.o
  CC      kernel/microkernel/k_pipe_util.o
  CC      kernel/microkernel/k_pipe_xfer.o
  CC      kernel/microkernel/k_nano.o
  CC      kernel/microkernel/k_server.o
  LD      kernel/microkernel/built-in.o
  CC      kernel/nanokernel/nano_fiber.o
  CC      kernel/nanokernel/nano_lifo.o
  CC      kernel/nanokernel/nano_fifo.o
  CC      kernel/nanokernel/nano_stack.o
  CC      kernel/nanokernel/nano_sys_clock.o
  CC      kernel/nanokernel/nano_context.o
  CC      kernel/nanokernel/nano_init.o
  CC      kernel/nanokernel/nano_sema.o
  CC      kernel/nanokernel/version.o
  CC      kernel/nanokernel/device.o
  CC      kernel/nanokernel/wait_q.o
  CC      kernel/nanokernel/nano_sleep.o
  CC      kernel/nanokernel/nano_timer.o
  CC      kernel/nanokernel/ring_buffer.o
  CC      kernel/nanokernel/errno.o
  CC      kernel/nanokernel/timeout_q.o
  LD      kernel/nanokernel/built-in.o
  LD      kernel/built-in.o
  CC      misc/printk.o
  LD      misc/debug/built-in.o
  CC      misc/generated/configs.o
  CC      misc/generated/sysgen/kernel_main.o
  LD      misc/generated/sysgen/built-in.o
  LD      misc/generated/built-in.o
  LD      misc/built-in.o
  LD      net/built-in.o
  CC      boards/arduino_101/pinmux.o
  CC      boards/arduino_101/board.o
  LD      boards/arduino_101/built-in.o
  LD      boards/built-in.o
  LD      ext/fs/built-in.o
  CC      ext/hal/qmsi/drivers/clk.o
  CC      ext/hal/qmsi/drivers/qm_flash.o
  CC      ext/hal/qmsi/soc/quark_se/drivers/power_states.o
  CC      ext/hal/qmsi/soc/quark_se/drivers/vreg.o
  CC      ext/hal/qmsi/drivers/qm_i2c.o
  CC      ext/hal/qmsi/drivers/qm_pwm.o
  CC      ext/hal/qmsi/drivers/qm_gpio.o
  CC      ext/hal/qmsi/drivers/qm_uart.o
  CC      ext/hal/qmsi/drivers/qm_dma.o
  CC      ext/hal/qmsi/drivers/qm_spi.o
  CC      ext/hal/qmsi/drivers/qm_pinmux.o
  LD      ext/hal/qmsi/built-in.o
  LD      ext/hal/built-in.o
  LD      ext/lib/crypto/built-in.o
  LD      ext/lib/built-in.o
  LD      ext/built-in.o
  CC      usb/usb_device.o
  CC      usb/class/cdc_acm.o
  LD      usb/class/built-in.o
  LD      usb/built-in.o
  LD      fs/built-in.o
  CC      arch/x86/core/cpuhalt.o
  CC      arch/x86/core/msr.o
  CC      arch/x86/core/dynamic.o
  CC      arch/x86/core/intconnect.o
  CC      arch/x86/core/excconnect.o
  CC      arch/x86/core/sys_fatal_error_handler.o
  AS      arch/x86/core/crt0.o
  AS      arch/x86/core/cache_s.o
  CC      arch/x86/core/cache.o
  AS      arch/x86/core/excstub.o
  AS      arch/x86/core/intstub.o
  AS      arch/x86/core/swap.o
  CC      arch/x86/core/thread.o
  CC      arch/x86/core/strtask.o
  CC      arch/x86/core/fatal.o
  LD      arch/x86/core/built-in.o
  CC      arch/x86/soc/quark_se/soc.o
  CC      arch/x86/soc/quark_se/soc_config.o
  CC      arch/x86/soc/quark_se/eoi.o
  CC      arch/x86/soc/quark_se/power.o
  AS      arch/x86/soc/quark_se/soc_power.o
  LD      arch/x86/soc/quark_se/built-in.o
  LD      arch/x86/built-in.o
  LD      arch/built-in.o
  CC      drivers/console/uart_console.o
  CC      drivers/console/ipm_console_receiver.o
  LD      drivers/console/built-in.o
  CC      drivers/gpio/gpio_api_compat.o
  CC      drivers/gpio/gpio_qmsi.o
  LD      drivers/gpio/built-in.o
  CC      drivers/i2c/i2c_qmsi.o
  LD      drivers/i2c/built-in.o
  CC      drivers/interrupt_controller/system_apic.o
  CC      drivers/interrupt_controller/loapic_intr.o
  CC      drivers/interrupt_controller/ioapic_intr.o
  LD      drivers/interrupt_controller/built-in.o
  CC      drivers/ipm/ipm_quark_se.o
  LD      drivers/ipm/built-in.o
  CC      drivers/pinmux/dev/pinmux_dev_qmsi.o
  LD      drivers/pinmux/dev/built-in.o
  LD      drivers/pinmux/built-in.o
  CC      drivers/pwm/pwm_qmsi.o
  LD      drivers/pwm/built-in.o
  LD      drivers/random/built-in.o
  CC      drivers/serial/uart_qmsi.o
  LD      drivers/serial/built-in.o
  CC      drivers/spi/spi_qmsi.o
  LD      drivers/spi/built-in.o
  CC      drivers/timer/loapic_timer.o
  CC      drivers/timer/sys_clock_init.o
  LD      drivers/timer/built-in.o
  CC      drivers/usb/device/usb_dc_dw.o
  LD      drivers/usb/device/built-in.o
  LD      drivers/usb/built-in.o
  LD      drivers/built-in.o
  CC      src/arduino/serial_print.o
  C++     src/arduino/variant.o
  CC      src/arduino/WInterrupts.o
/home/pymelab/CODK/CODK-M/x86-samples/Blink/src/arduino/WInterrupts.c: In function 'attachInterrupt':
/home/pymelab/CODK/CODK-M/x86-samples/Blink/src/arduino/WInterrupts.c:85:31: warning: passing argument 2 of 'gpio_init_callback' from incompatible pointer type [-Wincompatible-pointer-types]
  gpio_init_callback(&gpio_cb, callback, BIT(zephyrDescription[pin].zephyrPin1));
                               ^
In file included from /home/pymelab/CODK/CODK-M/x86-samples/Blink/src/arduino/WInterrupts.c:22:0:
/home/pymelab/CODK/zephyr/include/gpio.h:290:20: note: expected 'gpio_callback_handler_t {aka void (*)(struct device *, struct gpio_callback *, unsigned int)}' but argument is of type 'void (*)(void)'
 static inline void gpio_init_callback(struct gpio_callback *callback,
                    ^
  CC      src/arduino/wiring_analog.o
  CC      src/arduino/wiring.o
  CC      src/arduino/wiring_digital.o
  LD      src/arduino/built-in.o
  CC      src/arduino101_services/arduino101_services.o
  CC      src/arduino101_services/sharedmemory_com.o
  CC      src/arduino101_services/soc_ctrl.o
  CC      src/arduino101_services/cdcacm_serial.o
  LD      src/arduino101_services/built-in.o
  CC      src/blink.o
  LD      src/built-in.o
  AR      libzephyr.a
  LINK    zephyr.lnk
  SIDT    staticIdt.o
  LINK    zephyr.elf
  BIN     zephyr.bin
make[2]: se sale del directorio «/home/pymelab/CODK/CODK-M/x86-samples/Blink/outdir»
make[1]: se sale del directorio «/home/pymelab/CODK/zephyr»
pymelab@workstation:~/CODK/CODK-M/x86-samples/Blink$ 
```

```sh
pymelab@workstation:~/CODK/CODK-M/x86-samples/Blink$ sudo dfu-util -a x86_app -D outdir/zephyr.bin 
sudo: imposible resolver el anfitrión workstation
dfu-util 0.5

(C) 2005-2008 by Weston Schmidt, Harald Welte and OpenMoko Inc.
(C) 2010-2011 Tormod Volden (DfuSe support)
This program is Free Software and has ABSOLUTELY NO WARRANTY

dfu-util does currently only support DFU version 1.0

Opening DFU USB device... ID 8087:0aba
Run-time device DFU version 0011
Found DFU: [8087:0aba] devnum=0, cfg=1, intf=0, alt=2, name="x86_app"
Claiming USB DFU Interface...
Setting Alternate Setting #2 ...
Determining device status: state = dfuIDLE, status = 0
dfuIDLE, continuing
DFU mode device DFU version 0011
Device returned transfer size 2048
No valid DFU suffix signature
Warning: File has no DFU suffix
bytes_per_hash=1208
Copying data from PC to DFU device
Starting download: [##################################################] finished!
state(2) = dfuIDLE, status(0) = No error condition is present
Done!
pymelab@workstation:~/CODK/CODK-M/x86-samples/Blink$ 
```