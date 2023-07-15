小米7代游戏本的EFI

CPU：I7-7700HQ

OpenCore：0.9.3

Clover: r5151

# 解锁CFG LOCK
复制EFI_ru到空U盘里面，重命名为EFI，文件系统为FAT，然后重启电脑按F12启动，按‘ALT+=’选择‘CpuSetup’项，使用方向键移动到'0x3c'位置，改为‘00’，按下‘ALT+Q'保存修改'，重启

# 修改dvmt 64M
'SaSetup'项，位置；'0xDF',改为2

# macOS14 Sonoma
2023/06/09更新支持，EFI_14目录
WIFI、蓝牙 不可用
OpenCore 0.9.3
机型：MacbookPro15,2

# 支持的macOS版本
* macOS 14.0 Sonoma Beta
* macOS 13.3.1 Ventura
* macOS 12.6.5 Monterey
* macOS 11.7.6 Big Sur
* macOS 10.15.7 Catalina
* macOS 10.14.6 Mojave
* macOS 10.13.6 High Sierra

# 可用
* USB3.0
* 核显
* 音频（AppleALC alc_id 98)
* WIFI
* NVME/SATA 硬盘
* 蓝牙 （未测试隔空投送)
* 触控板
* CPU 睿频
* Type-c 视频输出，支持音频 （(需修改dvmt为64M)
* 睡眠（详见TIPS）(需修改dvmt为64M)
* 屏幕亮度调节 (需修改dvmt为64M)

# 不可用
* Nvidia GPU (永远不会被支持)
* 重启会卡，关机不会(clover版本可重启)


