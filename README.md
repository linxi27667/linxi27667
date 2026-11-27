# Hi, I'm Jeason.Liu (刘峻丞)

**Embedded Software & AIoT Systems Engineer** · `STM32` · `ESP32` · `FreeRTOS` · `4-Layer Industrial PCB` · `AI-Native Engineering`

专注 **MCU/RTOS 工业控制与 AIoT 智能硬件**，具备从 **原理图/四层 PCB 硬件协同 → 裸机/FreeRTOS 固件 → 4G/MQTT 云端 → Android 跨端 App** 的全链路独立闭环交付能力，同时深耕 **AI 上下文工程（Obsidian 工程知识库 + Agent Skills + 开源执行底座）**，用确定性规范与自动化门禁放大个人研发吞吐。

- 📍 **Location**: Guangzhou, China
- 🎓 **Education**: B.Eng. in Internet of Things Engineering, Guangzhou College of Commerce (Class of 2027)
- 🏆 **Awards**: 全国大学生嵌入式芯片与系统设计竞赛 **全国二等奖**（队长）、传智杯 AIoT **全国三等奖**（队长）等 **7 项国/省奖**
- 📫 **Contact**: `3081795804@qq.com`

---

## 🔧 Core Engineering Stack

| Domain | Technologies & Engineering Practices |
| :--- | :--- |
| **MCU & RTOS** | `C / C++` · `STM32F407 / F103 / G431` · `ESP32-P4 / S3 / C6` · `MSPM0` · `FreeRTOS` · `BSP-APP-TASK` 三层解耦架构 · 状态机 · 栈堆水位监控 |
| **Bus, Protocol & GUI** | `UART+DMA+FIFO` · `RS485` · `SPI / I2C / I2S / SDIO` · `MQTT (QoS1/幂等)` · `4G DTU/AT` · 自定义二进制帧 · `LVGL 9` · `MIPI-DSI/CSI` |
| **Hardware & EMC** | `嘉立创 EDA` · **四层工业控制板 PCB（454 器件 / 0-DRC）** · 24V 电源树与浪涌防护 · 光耦/P-MOS 高边/继电器驱动 · `J-Link / RTT / 示波器` |
| **Cloud & Cross-Platform App** | `Vue / H5 + Capacitor (Android Java 原生插件)` · `Node.js` · `ASP.NET Core` · `SQL Server / SQLite` · `MQTT Broker` · `Linux` |
| **AI-Native Engineering** | `Cursor / Claude Code / Antigravity / Codex` · **Obsidian 人机共读工程知识库（255+ 系统知识 / 24 份红线规则）** · **29 个垂直领域 Agent Skills** · `Node.js (CDP)` · `Rust (UIA)` |

---

## 🚀 Featured Projects

### 1. Embedded & AIoT Systems（嵌入式与智能硬件代表作）

| Project | Stack | Highlights |
| :--- | :--- | :--- |
| **[xiaozhi_p4](https://github.com/linxi27667/xiaozhi_p4)** | `ESP32-P4/C6/S3` `LVGL 9` `MCP` `ESP-DL` | **全国嵌入式竞赛二等奖**｜P4 中控 + C6 无线 + 三层 S3 分布式架构；大模型 MCP 受约束工具调用、1024×600 触控中控、二进制 MQTT 协议与并发内存峰值治理 |
| **[garden](https://github.com/linxi27667/garden)** | `ESP32-S3` `MQTT` `MCP` `Android 3D` | **「云亭智联」AIoT 智慧庭院**｜主从协同控制、本地火灾熔断安全闭环、语音/MCP 联动与 3D 数字孪生 |
| **[Mspm0_Track_Car](https://github.com/linxi27667/Mspm0_Track_Car)** | `MSPM0` `PID` `ESP-01S` `Python` | **5ms 实时闭环循迹车**｜灰度位置环 + 速度环、电机安全输出闸门与 Wi-Fi 远程实时调参上位机 |
| **[Esp32p4_Lvgl_Demo](https://github.com/linxi27667/Esp32p4_Lvgl_Demo)** / **[Lvgl_Smarthome_Sim](https://github.com/linxi27667/Lvgl_Smarthome_Sim)** | `ESP32-P4` `MIPI-DSI` `LVGL 9` | LVGL v9 移植与桌面端 UI 模拟器，支持设备模型单一事实源与无板级依赖快速迭代界面 |
| **[Esp32_Yinling_Care](https://github.com/linxi27667/Esp32_Yinling_Care)** / **[Esp32s3_Vision_Yolo](https://github.com/linxi27667/Esp32s3_Vision_Yolo)** | `ESP32-S3` `ESP-NOW` `YOLO` `Web` | 智慧养老多节点通信（小智 AI + ESP-NOW）与 ESP32-S3 双核边缘视觉检测实践 |

> **工业硬件与商业闭环（企业项目，源码未公开）**：
> - **STM32F407 多联举升机同步控制固件**：1～12 柱主从同固件、RS485 编码器高度闭环比例阀 PWM 调平、40mm 超差/急停本地安全停机、16 字节 CRC16 双通道帧与 Ymodem Bootloader。
> - **STM32F407 + 4G/GNSS/以太网/NFC 四层工业控制板**：`160×120 mm` 四层 PCB（454 器件、IEC 60664-1 220VAC 爬电净距 >=2.62mm、50Ω 零残桩射频、双轮 0-DRC 定版）。
> - **跨端工业移动 App（Android v2.9.8）**：Vue/H5 + Capacitor + Java 原生自动升级插件 + 41 仓实时库存镜像与电子签收双轨回写 ERP。

---

### 2. Embedded Architecture & Debug Tooling（底层架构与自研工具）

| Project | Stack | Highlights |
| :--- | :--- | :--- |
| **[Mcu_Bsp_Toolkit](https://github.com/linxi27667/Mcu_Bsp_Toolkit)** | `C` `STM32` `MSPM0` `FreeRTOS` | **BSP-APP-TASK 三层分离实践库**｜驱动层与原子业务层完全解耦，仅替换顶层即可在裸机时标切片与 FreeRTOS 任务间切换 |
| **[Pyqt_Rtt_Viewer](https://github.com/linxi27667/Pyqt_Rtt_Viewer)** | `Python` `PyQt5` `PyOCD` `SEGGER RTT` | **独立 SEGGER RTT 主机查看器**｜脱离官方 J-Link 工具，经 PyOCD 支持 DAPLink/ST-Link 读写 RTT 环形缓冲、彩色日志与实时波形 |
| **[Stm32g431_Freertos_Lab](https://github.com/linxi27667/Stm32g431_Freertos_Lab)** / **[Esp32s3_Contest_Lab](https://github.com/linxi27667/Esp32s3_Contest_Lab)** | `STM32G431` `ESP32-S3` `FreeRTOS` | 串口 `IDLE + DMA + RingBuffer` 通信范式与分层任务工程模板 |

---

### 3. AI-Native Engineering & Automation Infrastructure（AI 工程化与自动化底座）

| Project | Stack | Highlights |
| :--- | :--- | :--- |
| **[agent-browser-bridge](https://github.com/linxi27667/agent-browser-bridge)** | `Node.js` `CDP` `WebSocket` | **跨浏览器与桌面统一自动化执行底座（v0.8.0）**｜专用 Profile 身份校验、混合 `@ref` 语义快照、多 Agent 标签租约防冲突与增量 Diff，132 项单测通过 |
| **[agent-desktop](https://github.com/linxi27667/agent-desktop)** | `Rust` `Windows UIA` | **受控 Windows 桌面自动化引擎**｜原生 UIA 读写分离、非阻塞窗口恢复与单进程原子批量执行，245 项集成测试通过 |
| **[LexiGlass](https://github.com/linxi27667/LexiGlass)** | `Rust` `Tauri` `JavaScript` | 基于 Tauri 的轻量级跨端桌面效率工具 |

---

## 🧠 Engineering Philosophy

> **AI 是杠杆，架构边界与确定性验收才是护城河。**
>
> 日常研发维护一套 **Obsidian 人机共读知识库**（涵盖嵌入式软硬件底层、原厂芯片手册与整板逐颗原理图精讲、网络运维、制造系统与 Agent 工程 Spec）及 **29 个可执行 Agent Skills**，将“代码分层、ISR 边界、硬件 DRC 检查、实机验收清单”固化为机器可读约束——让 AI 懂工程，让自己把精力聚焦在系统设计、硬件协同与现场闭环。