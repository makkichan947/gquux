# gquux 内核

gquux 是一个现代化的、模块化的操作系统内核，设计用于多种架构平台。

## 特性

- 多架构支持 (x86_64, AArch64, RISC-V 64, PowerPC 64)
- 模块化设计
- 内存管理
- 进程调度
- 文件系统支持
- 网络协议栈
- 设备驱动框架

## 架构支持

- x86_64
- AArch64 (ARM64)
- RISC-V 64
- PowerPC 64

## 构建要求

- GCC 或兼容的交叉编译工具链
- GNU Make
- QEMU (用于测试)

## 构建

```bash
# 构建x86_64架构内核
./scripts/build.sh x86_64

# 构建其他架构
./scripts/build.sh aarch64
./scripts/build.sh riscv64
./scripts/build.sh powerpc
```

## 运行

```bash
# 在QEMU中运行x86_64内核
./scripts/run.sh x86_64

# 运行其他架构
./scripts/run.sh aarch64
./scripts/run.sh riscv64
./scripts/run.sh powerpc
```

## 目录结构

- `arch/` - 架构特定代码
- `drivers/` - 设备驱动
- `fs/` - 文件系统实现
- `include/` - 头文件
- `kernel/` - 内核核心代码
- `lib/` - 内核库
- `mm/` - 内存管理
- `net/` - 网络协议栈
- `sched/` - 调度器
- `scripts/` - 构建和运行脚本
- `sys/` - 系统服务
- `threads/` - 线程管理
- `usr/` - 用户管理

## 许可证

gquux 内核基于MIT许可证发布。
