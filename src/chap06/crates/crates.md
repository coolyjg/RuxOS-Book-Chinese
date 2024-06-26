
# 底层组件

本章节将对 RuxOS 中的底层组件进行介绍。

RuxOS 底层组件部分移植于 ArceOS，此外，也补充、完善了部分组件的实现。RuxOS 组件的设计理念来源于组件化操作系统的启发，底层组件提供了独立的、可跨操作系统复用的基础功能。

RuxOS 底层组件有如下特点：

- 充分解耦。不同组件之间代码完全独立，没有相互依赖。

- 开源共享。各个组件以独立的 Rust Crate 的形式存在，部分组件已由 r-core 社区发布到了 crates.io 中进行共享，丰富了组件化操作系统开源生态。

本章节中将对如下部分进行展开介绍：

- [硬件及 VirtIO 驱动封装](./drivers.md)。包括了 RuxOS 目前支持的各类驱动的简介。

- [操作系统开发相关数据结构](./kernel-tools.md)。包含了操作系统中用于开发的软件实现，用以简化调度器、内存分配器等的实现。

- [内存分配及调度算法实现](./algorithms.md)。包含了对 RuxOS 目前支持的内存分配算法以及任务调度算法的简介。

- [架构相关模块](./arch-related.md)。包含了 AArch64 架构上特殊驱动，以及设备树等内容。

- [文件系统及 IO 类](./fs-IO.md)。包含了 RuxOS 目前适配的各类文件系统，以及为上层定义的基于 Rust 标准库的 IO 相关 trait。

- [页表项及页表](./pte-pt.md)。涵盖了多种架构，RuxOS 实现的页表项定义及相关方法实现。

- [percpu类](./percpu.md)。提供了定义percpu数据结构的相关方法和宏。


