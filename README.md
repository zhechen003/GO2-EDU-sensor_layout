# GO2 EDU 3D 传感器布局与安装套件

本仓库提供一套面向 **Unitree GO2 EDU** 的 3D 传感器布局与安装结构，用于将 **Intel RealSense 深度相机** 和 **Livox Mid-360 激光雷达** 集成到机器人头部区域。

设计以轻量、稳固、易维护为目标，采用模块化结构与快拆装接口，便于根据任务需求快速安装、移除或更换传感器组件。

## 功能特点

- **双传感器集成**：为 RealSense 深度相机与 Mid-360 激光雷达提供专用安装位。
- **3D 感知布局**：兼顾相机视场、激光雷达视野以及与 GO2 EDU 机身的空间关系。
- **模块化设计**：相机支架、雷达支架、头部安装件和连接转接件可独立拆装与更换。
- **快拆装能力**：基于快拆转接结构，方便在调试、运输和不同任务载荷之间快速切换。
- **可制造文件齐全**：提供 SolidWorks 源文件、STL 打印文件及部分 STEP 交换格式文件。

## 文件说明

| 文件 | 用途 |
| --- | --- |
| `Go2EDU-head.SLDPRT` / `Go2EDU-head.STL` | GO2 EDU 头部/主体安装件 |
| `camera_support.SLDPRT` / `camera_support.STL` | 相机支撑结构 |
| `realsense_support.SLDPRT` / `realsense_support.STL` | RealSense 相机专用安装件 |
| `lidarsupport1.SLDPRT` / `lidarsupport1.STL` | Mid-360 激光雷达安装支架 |
| `arc-swiss.SLDPRT` / `arc-swiss.STL` | 快拆转接件 |
| `backborad1.SLDPRT` / `backborad1.STEP` | 后部连接板/安装板 |

## 安装建议

1. 使用 `Go2EDU-head` 将整套结构固定到 GO2 EDU 对应安装位置。
2. 将 `arc-swiss` 快拆转接件与主体安装件连接，并确认锁紧可靠。
3. 按传感器类型分别安装 `realsense_support` 与 `lidarsupport1`。
4. 安装 RealSense 相机和 Mid-360 后，检查其视野是否被支架、线缆或机身遮挡。
5. 整理传感器线缆并预留活动余量，确认机器人运动时不会发生干涉。

> 请在开机运行前复核紧固件、载荷重心、线缆固定和传感器视野。实际安装尺寸、紧固件规格及线缆走线应以所使用的 GO2 EDU、RealSense 和 Mid-360 型号为准。

## 使用与制造

- 可直接使用 `.STL` 文件进行 3D 打印验证。
- 可使用 SolidWorks 打开 `.SLDPRT` 文件进行尺寸调整或二次设计。
- `backborad1.STEP` 可用于与其他 CAD 软件或总装模型交换。

## 适用场景

- 室内外自主导航与建图
- 多传感器融合定位
- 三维环境感知与避障
- GO2 EDU 研究、教学与原型开发

## 许可与使用说明

本仓库用于分享 GO2 EDU 的传感器布局与安装结构。使用、修改或制造前，请自行确认其与机器人、传感器及周边设备的机械兼容性与使用安全。

