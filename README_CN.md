# GO2 EDU 3D 传感器布局与快拆安装套件

<p align="center">
  <img src="assets/go2-edu-sensor-layout.png" alt="GO2 EDU RealSense 相机与 Mid-360 激光雷达传感器布局" width="760">
</p>

<p align="center">
  <a href="README.md">English</a> · <strong>中文</strong>
</p>

本仓库提供一套面向 **Unitree GO2 EDU** 的模块化 3D 传感器布局与安装套件，将 **Intel RealSense 深度相机** 和 **Livox Mid-360 激光雷达** 集成到紧凑的头部安装结构中。

设计将相机支架、雷达支架、快拆转接件和 GO2 EDU 主安装结构分离，方便在开发调试、运输或切换不同任务载荷时快速安装、移除和重新配置传感器。

> For English documentation, see [README.md](README.md).

## 功能特点

- **双传感器集成**：为 RealSense 深度相机与 Mid-360 激光雷达分别提供专用安装位。
- **面向 3D 感知的布局**：兼顾相机视场、激光雷达覆盖范围，以及与机器人机身之间的空间间隙。
- **模块化设计**：相机、雷达、头部安装件和转接件均可独立维护或更换。
- **快拆装能力**：通过快拆转接件，在测试、运输和任务载荷切换时快速完成装卸。
- **可制造文件齐全**：提供 SolidWorks 源文件、3D 打印 STL 文件及 STEP 交换文件。

## 文件说明

| 文件 | 用途 |
| --- | --- |
| `Go2EDU-head.SLDPRT` / `Go2EDU-head.STL` | GO2 EDU 头部 / 主安装结构 |
| `camera_support.SLDPRT` / `camera_support.STL` | 相机支撑结构 |
| `realsense_support.SLDPRT` / `realsense_support.STL` | RealSense 相机安装件 |
| `lidarsupport1.SLDPRT` / `lidarsupport1.STL` | Mid-360 激光雷达安装支架 |
| `arc-swiss.SLDPRT` / `arc-swiss.STL` | 快拆转接件 |
| `backborad1.SLDPRT` / `backborad1.STEP` | 后部连接板 / 安装板 |

## 安装概要

1. 使用 `Go2EDU-head` 将主结构固定到 GO2 EDU 的对应安装位置。
2. 安装并可靠锁紧 `arc-swiss` 快拆转接件。
3. 将 `realsense_support` 和 `lidarsupport1` 装到对应安装位。
4. 安装 RealSense 相机与 Mid-360 后，检查支架、线缆和机身不会遮挡传感器视野。
5. 整理并固定传感器线缆，为机器人运动预留足够余量，避免发生干涉。

## 已采用本构型的研究工作

本套传感器构型已用于以下 GO2 研究系统：

- **[SCAN-Planner](https://github.com/wuyi2121/SCAN-Planner)** —— 面向长距离四足机器人导航的空间碰撞感知局部规划方法。[论文（arXiv:2606.19555）](https://arxiv.org/abs/2606.19555)
- **[TravExplorer](https://github.com/wuyi2121/TravExplorer)** —— 面向跨楼层具身探索的可通行性感知三维规划方法。[论文（arXiv:2605.19958）](https://arxiv.org/abs/2605.19958)

## 制造与修改

- 使用 `.STL` 文件进行 3D 打印验证。
- 使用 SolidWorks 打开 `.SLDPRT` 文件，按需调整尺寸或接口。
- 使用 `backborad1.STEP` 与其他 CAD 软件或总装模型交换后部连接板。

## 安全与兼容性

运行机器人前，请检查紧固件、线缆走线、载荷重心和传感器视野。机械尺寸、紧固件规格、线缆走线和电气接口应以实际使用的 GO2 EDU、RealSense 和 Mid-360 硬件为准。
