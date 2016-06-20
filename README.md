# ath9k_ocb_linux_4.7.rc3
This repository contains a modification of linux 4.7.rc3 ath9k driver. This modification support OCB mode for atheros cards which it use the ath9k driver.

##Introduction
The source of the kernel 4.7.rc3 is [kernel 4.7](https://github.com/torvalds/linux) and the specific commit
is [5edb564](https://github.com/torvalds/linux/releases/tag/v4.7-rc3)

It had only been modified the files:
- drivers/net/wireless/ath/ath9k/ani.c
- drivers/net/wireless/ath/ath9k/ath9k.h
- drivers/net/wireless/ath/ath9k/common-init.c
- drivers/net/wireless/ath/ath9k/debug.c
- drivers/net/wireless/ath/ath9k/htc_drv_init.c
- drivers/net/wireless/ath/ath9k/hw.c
- drivers/net/wireless/ath/ath9k/hw.h
- drivers/net/wireless/ath/ath9k/init.c
- drivers/net/wireless/ath/ath9k/main.c
- drivers/net/wireless/ath/ath9k/recv.c
- drivers/net/wireless/ath/regd.c

And the changes that it had been made,it was following the same changes that [lisovy](https://github.com/lisovy) had made in the
repository [CTU-IIG/802.11p-linux](https://github.com/CTU-IIG/802.11p-linux/commit/bf45e0160af428dac8893e48d506ac428fed16b2).

##Instructions

Copy the folder "drivers" in your onw kernel (4.7.rc3) it is the only way to install them. After this, you can compile the kernel
with the properly configuration.
