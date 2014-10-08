Openwrt-MR12
============

Bringup Repo for the Cisco Meraki MR12 on the latest OpenWRT Nightlies


About
-----
Based on OpenWRT CHAOS CALMER r42690. May or may not work on newer revisions.

Building
--------
git sync, copy files on top of build dir, menuconfig && kernel_menuconfig to mr12, build, and enjoy

Booting
-------
tftpboot 0x81000000 openwrt-ar71xx-generic-mr12-initramfs-uImage.bin; bootm

To Do
-----
* Bring up the 2nd NIC (Not on SPI?)
* Use Proper NIC MAC Addresses (We are at the right addr, but does not match MAC on device)
* Test Sysupgrade/Flashable Images
* Possibly More?

Notice
------
I have only tested with with TFTP booting and NOT flashing to the flash. No promises this won't break everything!