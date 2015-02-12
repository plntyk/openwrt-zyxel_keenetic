# openwrt-zyxel_keenetic

This repository contains patches to enable OpenWrt on Zyxel Keentic series.

The original series has several issues and does not apply to current trunk.

This repo intends to fix this.

Original Source Forum: http://4pda.ru/forum/index.php?showtopic=551476

Original Source Web Repo: http://s-trace.url.ph/files/ZyXEL_Keenetic_Series/OpenWRT/47/svn_47.diff

OpenWrt Forum: https://forum.openwrt.org/viewtopic.php?id=55733

Patch on openwrt-devel not committed:
https://lists.openwrt.org/pipermail/openwrt-devel/2014-February/024088.html


TODO:
- Separate optional and necessary features
- create patch series for Kernel/userland/image creation
- fix coding issues

DONE:
- packages contains posixovl and davfs2 that were integrated into Zyxel Keenetic series
- Separation into single files
- tools/zyimage series : 01a,01b complete
