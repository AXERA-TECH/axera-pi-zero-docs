# AX Pi Zero 概述

## 购买方式

- [淘宝-网讯智能](https://item.taobao.com/item.htm?spm=a1z10.1-c-s.w4001-25302603957.1.44c94a94Ef0oMT&id=766038092712&scene=taobao_shop&skuId=5626935563671)

## 爱芯派Zero

**爱芯派Zero（AXera-Pi Zero）** 搭载爱芯元智第四代智能视觉芯片 **[AX620Q](https://www.axera-tech.com/Product/127.html)** ，该芯片集成新一代智眸 4.0 AI-ISP，最高支持 5MP@30fps 实时真黑光，同时集成新一代通元 4.0 高性能、场景优化的 NPU 引擎，使得产品在低功耗、高画质、智能处理和分析等方面行业领先。

爱芯派 Zero 提供稳定易用的 SDK 软件开发包，方便用户低成本评估、
二次开发和快速量产。帮助用户在智能家居应用和其他 AIOT 项目中发挥更大的价值。

已支持 Sensor
- **SC450AI**
- **SC200AI**

![](./media/10.png)

## 规格
<title>Document</title>

| AXera-Pi Zero | 规格 | 
| --- | --- |
| SoC | AX620Q |
| 处理器 | 2 x Arm Cortex-A53@1.2GHz |
| ISP能力 | 最大支持 5MP@30fps<br />AI-ISP&T-ISP<br />支持 3A<br />AI-3DNR<br />AIRLTM<br />两帧HDR</li></li>图像增强<br />去雾功能<br />鱼眼矫正 |
| AI能力 | 9.6TOPs@INT4<br />2.4TOPs@INT8 |
| 操作系统 | Linux |
| 深度学习框架 | 支持 ONNX、PyTorch、Caffe、PaddlePaddle 等模型部署 |
| 视频编码能力 | H.264/H.265<br />5MP@30fps+1080P@30fps+720P@30fps |
| 视频解码能力 | H.264<br />1080P@60fps |
| 图片编解码能力 | JPEG<br />编码 5MP@40fps<br />解码 1080P@60fps |
| 其他功能 | 支持 CBR/VBR/AVBR/CVBR 多种码率控制模式<br />支持 8 个 ROI 编码 |
| 内存 | SIP 256MiB LPDDR4X |
| 存储 | SPI NAND 256MiB |
| 接口 | 1 x MIPI CSI 4-lane<br />1 x 10/100 RJ45 网口<br />1 x USB2.0<br />1 x TF 卡槽<br />RTC 电池接口<br />GPIO接口<br />2 x 按键（BOOT、RESET）<br />1 x LED<br />DC 5V（USB 供电） |
| 环境 | 工作温度：-40°C ~ 85°C<br /> |
| 功耗 | 1.2W |
| 结构 | 65 × 30 mm |

## 特点
<p><font size="4"><b>高性价比</font></b></p>
<ul>
<li>内置双核 64 位高性能 ARM CPU;</li>
<li>内置 AI 算力 9.6 TOPs INT4 或 2.4 TOPs INT8;</li>
<li>内置 AI-ISP，支持 500 万像素，支持 3A、3DNR、HDR、图像增强、去雾功能和鱼眼矫正算法;</li>
<li>内置 256MB LPDDR4、Audio Codec、ePHY。</li>
</ul>

<font size="4"><b>易部署</font></b>
<ul>
<li>USB Type-C 供电&调试;</li>
<li>Linux 系统;</li>
<li>丰富扩展接口;</li>
<li>软硬件资料丰富，开发者社区活跃。</li>
</ul>

## 资料汇总

### 网盘资料

- 网盘资料包含 **硬件参考设计**、**预编译固件(*.axp)**、**固件烧写软件(AXDL)**、**相关驱动** 等文件；
- [百度网盘(提取码：Zero)](https://pan.baidu.com/s/1ZhK5TAt4H6BPRn4bDA1oXA)

### 社区资料

- [应用层示例](https://github.com/AXERA-TECH/ax620q_bsp_sdk/tree/zero)，包含以下内容

    - FRTDEMO，完整的IPC应用软件，实现 Web 管理、主副码流控制、RTSP拉流、黑光全彩自动切换(AI ISP)、智能算法(SKEL)、JPEG抓拍、视频录制保存等功能及其源码；
    - Samples，各功能模块单一示例，包含了 VIN、VO、VENC、VDEC、SKEL、NPU、VIN_IVPS_ENGINE_VENC_RTSP 等等。

- [NPU示例](https://github.com/AXERA-TECH/ax-samples)，包含以下内容

    - 主流的视觉类深度学习算法模型示例，包含了 分类、检测、人体关键点、实例分割、单目深度估计 等等。

- QQ技术交流群

    - 139953715

## 应用场景
<ul>
<li>智能AIOT</li>
<li>智能机器人</li>
<li>智能家居</li>
<li>智慧教育</li>
<li>智慧社区</li>
<li>智能制造</li>
</ul>