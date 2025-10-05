# postmarketOS on Redmi 8 (olive)

> [!CAUTION]
> Your warranty is now void.
I am not responsible for bricked devices, dead SD cards, thermonuclear war,
or you getting fired because the alarm app failed.
Please do some research if you have any concerns about features included in this ROM before flashing it!
YOU are choosing to make these modifications, and if you point the finger at me for messing up your device,
I will laugh at you. 

## System specs:
| Part | Component |
|-----:|-----------|
|CPU|Octa-core (4x1.95 GHz Cortex-A53 & 4x1.45 GHz Cortex A53)|
|Chipset|Qualcomm Snapdragon 439|
|GPU|Adreno 505|
|Storage|32/64GB eMMC 5.1|
|RAM|3/4GB|
|External Storage|MicroSDXC (up to 128GB)|
|OS|Android 9 (Launch) - Android 10|
|Other|WiFi (2.4GhZ), GPS, Bluetooth 4.2|

**Full specs:** https://www.gsmarena.com/xiaomi_redmi_8-9800.php

## Working:
● Flashing

● USB Networking (Works, but after a few seconds crashes kernel)

● Screen

● WiFI (Connect using "sudo nmtui")

● FDE

## Broken:
● Audio (except Volume Control)

● SDcard/Sim

● Accelerometer

● Bluetooth

● Touchscreen

## Device source:
● [Device tree](https://github.com/mi-sdm439/android_device_xiaomi_olive)

● [Kernel package](https://gitlab.postmarketos.org/postmarketOS/pmaports/-/tree/master/device/downstream/linux-xiaomi-olive)

## Installing postmarketOS:
1. pmbootstrap init (choose channel v24.06)
2. pmbootstrap install --fde --add unl0kr
3. pmbootstrap flasher flash_kernel
4. pmbootstrap flasher flash_rootfs --partition=userdata
5. Reboot

**So, that's it.**

## Additional links:
● Redmi 8 postmarketOS wiki page: https://wiki.postmarketos.org/wiki/Xiaomi_Redmi_8_(xiaomi-olive)

● Channel about running Linux on olive: https://t.me/xiaomi_sdm439_olives_linux
