# openwrt-zyxel_keenetic

This repository contains patches to enable OpenWrt on Zyxel Keentic series.

The original series has several issues and does not apply to current trunk.

This repo intends to fix this.

Original Source Forum: http://4pda.ru/forum/index.php?showtopic=551476

Original Source Web Repo: http://s-trace.url.ph/files/ZyXEL_Keenetic_Series/OpenWRT/47/svn_47.diff

OpenWrt Forum: https://forum.openwrt.org/viewtopic.php?id=55733

Patch on openwrt-devel not committed:
https://lists.openwrt.org/pipermail/openwrt-devel/2014-February/024088.html

Initially these are p0 patches - so git apply -p0 <patchname>

Order to apply:
- 01 (tools/zyimage)
- 10-19 add .dts files
- 20 add pins to mt7620dtsi
- 21 **(userspace does not apply atm)**
- 22,23 profiles
- 24 **(Image generation does not apply)**

TODO:
- Separate optional and necessary features
- create patch series for Kernel/userland/image creation
- fix coding issues
- convert to -p1 patches

DONE:
- packages contains posixovl and davfs2 that were integrated into Zyxel Keenetic series
- Separation into single files
- tools/zyimage series : 01a,01b complete
- fix some whitespace issues
