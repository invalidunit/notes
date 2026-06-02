# 扩容 OpenWrt（ext4）

## 准备工作

检查更新

  opkg update

安装必要包

  opkg install parted losetup resize2fs

## 开始扩容

进入 parted 确认需要扩容的序号

  parted

  print

退出，然后将剩余空间分配给 2

  parted -s /dev/mmcblk0 resizepart 2 100%

  losetup /dev/loop0 /dev/mmcblk0p2

  resize2fs -f /dev/loop0
