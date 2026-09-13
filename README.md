<div align="center">

# PokeballPlus for PC

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![.NET 8.0](https://img.shields.io/badge/.NET-8.0-512BD4.svg)](https://dotnet.microsoft.com/zh-cn/download/dotnet/8.0)
[![ViGEm](https://img.shields.io/badge/ViGEm-1.22.0-0078D4.svg)](https://github.com/nefarius/ViGEmBus)

**语言 / Language**  
[简体中文](#简体中文) | [English](#english)

</div>

---

<a id="简体中文"></a>
## 简体中文

### 项目简介
本软件基于 [Pokeballplus4Windows](https://github.com/原项目地址) 项目（MIT 许可）二次开发，基于 C# / .NET 8.0 构建，可将任天堂 Switch 精灵球控制器转换为 Windows 平台的 XInput 游戏手柄与高精度空气鼠标。

### 运行依赖
- .NET 8.0 Desktop Runtime 运行库
- ViGEm Bus Driver v1.22.0 虚拟手柄驱动

### v2.0 核心功能
1. 采用非单文件编译，彻底修复鼠标指针闪烁 bug
2. 新增「虚拟摇杆」鼠标模式：基于重力加速度传感器模拟摇杆控制逻辑，自动适配传感器底噪与死区
3. 新增「激光笔」空气鼠标模式：六轴陀螺仪+加速度传感器方案，实现类似 LG Magic Remote 的高精度指针控制
4. 双模式切换逻辑：按住红色按键+摇晃切换两种鼠标模式；直接摇晃切换手柄/鼠标模式
5. 多档位节电超时，超时自动断连设备强制休眠
6. 自动摇杆校准功能，转动摇杆即可自动居中修正漂移
7. 为模式切换操作增加 Windows 原生 Toast 通知机制，切换成功后自动弹出提示，用户无需手动操作即可确认当前状态
8. 中英双语界面，支持即时切换
9. 配置文件持久化保存用户设置
10. 修复并优化原项目多处潜在 bug 与设计问题

### 使用说明
1. 安装 .NET 8.0 Runtime 与 ViGEm Bus Driver 驱动
2. 解压压缩包，运行主程序 exe
3. 通过蓝牙连接 Poké Ball Plus 控制器，软件将自动识别设备

[⬆ 返回顶部](#pokeballplus-for-pc)

---

<a id="english"></a>
## English

### Introduction
This software is a secondary development based on the [Pokeballplus4Windows](https://github.com/原项目地址) project (MIT License), built with C# / .NET 8.0. It converts the Nintendo Switch Poké Ball Plus controller into an XInput gamepad and high-precision air mouse for Windows.

### Requirements
- .NET 8.0 Desktop Runtime
- ViGEm Bus Driver v1.22.0

### Key Features in v2.0
1. Non-single-file compilation to fully fix the mouse cursor flickering bug
2. New "Virtual Joystick" mouse mode: accelerometer-based joystick control logic with auto-adaptive noise floor and dead zone
3. New "Laser Pointer" air mouse mode: 6-axis gyro + accelerometer solution for LG Magic Remote-like high-precision pointer control
4. Dual mode switching: hold red button + shake to toggle two mouse modes; shake directly to switch gamepad/mouse mode
5. Configurable power-saving timeout, auto disconnect and force sleep after idle
6. Automatic joystick calibration — rotate the stick to auto-center and correct drift
7. Added native Windows Toast notification for mode switching operations. A pop-up prompt appears automatically upon successful switching, so users can confirm the operation status without checking it manually
8. Bilingual (Chinese / English) interface
9. Configuration file for persistent user settings
10. Fixed and optimized multiple potential bugs and design flaws in the original project

### Usage
1. Install .NET 8.0 Runtime and ViGEm Bus Driver
2. Extract the package and run the executable
3. Connect your Poké Ball Plus via Bluetooth; it will be automatically recognized

[⬆ Back to Top](#pokeballplus-for-pc)
