## ChangeLog ISVP-3.9.0-2016.12.9
----------

* [Toolchain]更新r2.3.3版本：优化SIMD128编译；添加nostripped uclibc库；修复uclibc busybox nslookup的bug；添加mips-linux-uclibc-gnu-XXX的uclibc程序编译方式
* [rootfs]更新busybox,lib，添加logcat到参考rootfs
* [u-boot]优化DDR 参数，提高效率(重要)；添加Lite Version芯片编译配置（T10L以及T20L请使用Lite的配置）；添加SPI Nor Flash FM25Q64A支持；SD卡自动更新添加CRC校验
* [kernel]优化ISVP的默认配置，优化系统的稳定性及效率；gmac驱动添加ethtool接口
* [Sensor]添加了ov2710,ov4689,gc2023,imx322,sc2135,jxf22,bg0806的支持以及效果文件
* [ISP]T20添加MIPI-CSI支持，修复驱动自定义功能的bug
* [Encoder]修复码流控制算法的一些问题
* [Audio]优化AEC，添加ADPCM编解码支持
* [Carrier]添加JPEG抓拍功能
* [Doc]添加T20开发板Medlar及Bull的说明文档，更新FAQ，更新三方库编译文档等

注：

* 本次更新可以兼容上个版本的内核(Ver.3.8.0)，建议更新config配置(defconfig)
* 建议更新Toolchain及rootfs(uclibc)，修复uclibc的bug以及支持uclibc gdbserver。新版本Toolchain及rootfs兼容旧版本，即旧版本可以正常使用
