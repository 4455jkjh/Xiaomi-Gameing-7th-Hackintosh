小米7代游戏本的EFI

CPU：I7-7700HQ

OpenCore：0.9.1

# 解锁CFG LOCK
复制EFI_ru到空U盘里面，重命名为EFI，文件系统为FAT，然后重启电脑按F12启动，按‘ALT+=’选择‘CpuSetup’项，使用方向键移动到'0x3c'位置，改为‘00’，按下‘ALT+Q'保存修改'，重启

# 支持的macOS版本
* macOS 13.3.1 Ventura
* macOS 10.15 Catalina

# 可用
* USB3.0
* 核显
* 音频（AppleALC)
* WIFI
* NVME/SATA 硬盘
* 蓝牙,支持隔空投送
* Type-c 视频输出，支持音频 （详见TIPS）
* 触控板

# 不可用
* Nvidia GPU (永远不会被支持)
* 重启会卡，关机不会
* 睡眠（详见TIPS）
* 无法调节屏幕亮度

# TIPS
* 在boot-args添加参数-wegnoegpu可以解决睡眠问题，但是这样type-c接口无法连接显示器，只能二选一

