# 第九章：文件系统

## 本章概要

之前我们只能在内核代码中硬编码跑什么用户程序，现在我们实现一个简单的终端，可以由我们自己输入跑什么程序！这说明我们要同时将多个程序组成的镜像链接进内核，于是我们使用文件系统来打包镜像，在内核中解析镜像取出单个用户程序。

本章你将会学到：

- 为文件系统开发最简单的设备驱动
- 如何实现线程的阻塞与唤醒
- 用缓冲区描述标准输入，并利用线程阻塞提高 CPU 利用率
- 实现用户态终端程序

## 参考资料
1. [rCore 文件系统分析](figures/rcore_fs_analysis.pdf)
2. [xv6 文件系统分析](figures/xv6_fs_analysis.pdf)
