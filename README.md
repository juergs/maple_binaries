# maple_binaries
Locutus MapleMini Firmware Variante:
maple_mini_boot20.bin is bootloader over serial for stm32flash 
stm32flash -w maple_mini_boot20.bin /dev/ttyUSB0

MapleCULx4.bin flash after bootloader ...

Result version for a-culfw:
V 1.24.02 a-culfw Build: private build (unknown) MapleCULx4_03 (F-Band: 868MHz)

sources from: https://github.com/heliflieger/a-culfw/tree/master/culfw or from
https://github.com/Telekatz/a-culfw/tree/MapleSduino/culfw
Actual Version is 1.26.08

How-To compile with WSL:
https://forum.fhem.de/index.php/topic,106278.msg1037755.html#msg1037755

Fhem-Thread:
https://forum.fhem.de/index.php/topic,80872.msg729752.html#msg729752
https://forum.fhem.de/index.php/topic,60458.msg621959.html#msg621959

Reach Windows folder from WSL in this manner:
/mnt/d/Work_FHEM/_maple_sduino/_projects/a-culfw-telekatz.1.26.08/a-culfw/culfw/Devices/MapleCUN

Edit Makefile to use right version:


- *CC=/mnt/d/Work_Fhem/gcc-arm-none-eabi-6-2017-q2-update-linux/bin/arm-none-eabi-gcc*

- *OBJCOPY=/mnt/d/Work_Fhem/gcc-arm-none-eabi-6-2017-q2-update-linux/bin/arm-none-eabi-objcopy*

- *SIZE=/mnt/d/Work_Fhem/gcc-arm-none-eabi-6-2017-q2-update-linux/bin/arm-none-eabi-size*

[code and compiling] (https://github.com/juergs/a-culfw-telekatz-MapleCUL2x)

Some more infos could be found there:
https://wiki.fhem.de/wiki/MapleCUN#Bootloader_flashen

![Image of MapleCUL2x](https://github.com/juergs/maple_binaries/blob/main/Eigenbau_MapleCUL%20_MapleCUN.png)

![Image of MapleCUL2x-Schmatic](https://github.com/juergs/maple_binaries/blob/main/Locutus_mapleculx2_schematic.png)

![Image of MapleCUL2x-Pinout_differences](https://github.com/juergs/maple_binaries/blob/main/MapleCul_vs_MapleSDuino_Pinzuordnung.png)

