# archlinux-arm-mainline-catdrive
## Introduction

Essential patches &amp; tweaks on Arch Linux ARM mainline kernel for Catdrive. 

适用于猫盘 Arch Linux ARM主线内核(linux-aarch64)的修改/调教。

Contains a patched Device Tree for Marvell 88E1512 PHY to bypass "CRC Error" and to set desired LED function.

 包含一份为Marvell 88E1512网卡芯片修改过的设备树，以规避“CRC Error”错误并设置网口LED功能。

A aw2013 DKMS driver is also included to enable LED function missing on the mainline kernel.

为了在主线内核中启用LED功能，一份aw2013的DKMS驱动也已经随代码提供。

## WARNING

- To let DKMS driver function properly, you **MUST** install ```dkms``` package manually.

- 为了让DKMS驱动发挥作用，您**必须**手动安装```dkms```软件包。

- This patch is aimed for Arch Linux ARM with mainline kernel. Nothing can be guaranteed under other circumstances (e.g. arch with linux-espressobin kernel, or other distributions).  ***USE AT YOUR OWN RISK!***

- 这份修补为带有主线内核(linux-aarch64)的Arch Linux ARM制作。在其他环境下（比如带有linux-espressobin内核的Arch，或是其他发行版），该补丁可能无法生效。***使用前请三思！***

## Credits

@hanwckf (https://github.com/hanwckf) for initial mainline driver code.
