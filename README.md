小米7代游戏本的EFI

CPU：I7-7700HQ

OpenCore：0.9.1

# BUG
* 重启会卡，关机不会

# 解锁CFG LOCK
复制EFI_ru到空U盘里面，重命名为EFI，文件系统为FAT，然后重启电脑按F12启动，按‘ALT+=’选择‘CpuSetup’项，使用方向键移动到'0x3c'位置，改为‘00’，按下‘ALT+Q'保存修改'，重启

# 支持的macOS版本
* macOS 13.3.1 Ventura
* macOS 10.15 Catalina

# 可用
* USB3.0
* 睡眠
* 核显
* 音频（AppleALC)
* WIFI
* NVME/SATA 硬盘
* 蓝牙
* Type-c 视频输出，支持音频

# 不可用
* 触控板
* Nvidia GPU (永远不会被支持)

