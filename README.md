# proj148-RDMA-Driver-Rust-eBPF

### 项目名称
基于Rust和eBPF实现RDMA内核模块、驱动

### 支持单位
DatenLord

### 项目描述

Rust是新一代高级编程语言，Rust的安全特性使其在系统编程领域有独特的优势，目前Linux内核社区，特别是Linux驱动相关的部分开始接受Rust的实现。

eBPF是Linux内核的新特性，方便用户在内核里安全运行自定义的逻辑，eBPF在网络、安全、可观测性方面已经有了很多应用，在Linux驱动方面eBPF也正在尝试。

RDMA是高性能网络协议栈，常用于高性能计算领域。RDMA的驱动包括通用的内核模块OFED和不同厂商适配其RDMA硬件网卡的驱动。

本项目要求基于RDMA和eBPF实现RDMA驱动：
- 一方面对RDMA通用内核模块OFED做封装（建议OFED的封装采用Rust实现），用于支持eBPF调用；
- 另一方面对底层硬件进行封装实现硬件抽象层HAL（建议HAL采用Rust实现），用于是指eBPF调用。

### 所属赛道

2022全国大学生操作系统比赛的“OS功能挑战”赛道

### 参赛要求

- 熟悉Rust，特别是Rust内核编程
- 熟悉eBPF

### 项目导师

王璞

* github https://github.com/datenlord
* email pwang7@foxmail.com

### 难度

高难度

### 特征

- 建议基于Linux内核5.10以上版本

### License
- GPL-2.0 License

## 预期目标

- 基于Rust实现RDMA通用内核模块OFED的封装，以及RDMA底层硬件抽象层HAL的封装
- 基于eBPF实现RDMA驱动
