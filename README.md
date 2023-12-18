# Custom Firmware for locked tl-mr3020 

## ``setenv ipaddr 192.168.1.1``

## ``setenv serverip 192.168.1.100``

## ``tftpboot 0x80000000 openwrt-ar71xx-generic-tl-mr3020-v1-squashfs-factory.bin``

## ``erase 0x9f020000 +0x3c0000``

## ``cp.b 0x80000000 0x9f020000 0x3c0000``

## ``bootm 9f020000``

# References:

* https://www.mdsec.co.uk/2015/09/an-introduction-to-hardware-hacking-the-ripe-atlas-probe/

* https://sizeof.cat/post/from-a-ripenet-probe-to-openwrt-router/
