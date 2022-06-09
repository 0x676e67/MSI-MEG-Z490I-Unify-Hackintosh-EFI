[![OpenCore](https://img.shields.io/badge/OpenCore-0.8.1-yellowgreen)](https://github.com/zf1976/MSI-MEG-Z490I-Unify-Hackintosh-OC-EFI/releases/tag/OC-0.7.1)
[![macOS](https://img.shields.io/badge/macOS-12.4-orange)](https://www.apple.com/macos/catalina/)
[![MODEL](https://img.shields.io/badge/Model-Z490I-blue)](https://tw.msi.com/Motherboard/MEG-Z490I-UNIFY/)
[![BIOS](https://img.shields.io/badge/BIOS-7C77v19-brightgreen)](#)

<img src="/img/BD00B09E-EE51-49BF-AD26-4E10A52D512D.png"/>

## i9 10850K + MSI-MEG-Z490I-Unify 核显 独显 Hackintosh EFI

> Wi-Fi蓝牙驱动只适配最新版Monterey，使用另外两个版本系统需要自行更换蓝牙、网卡驱动等等(各大版本使用驱动不兼容)，支持OTA升级，建议使用镜像升级。
- Catalina 10.15.x
- BugSur 11.x
- Monterey 12.4

---


### 电脑配置

| 规格     | 详细信息                                     |
| -------- | ---------------------------------------- |
| 机箱 | MQ6             |
| 电源 | 益衡7660B             |
| CPU散热 | AXP120             |
| 主板型号 | MSI-Z490I-Unify             |
| 处理器   | Intel Core i9 10850K       |
| 内存     | Asgard 64GB 2x32GB DDR4 3000Mhz                 |
| 硬盘     | WDS500G3X0C-00SJG0 512GB M.2 NVMe                  |
| 显卡 | ASRock Radeon RX 5500 XT Challenger ITX 8G 1717MHz 8GHz GDDR6                            |
| 板载网卡 | 英特尔® Wi-Fi 6 AX201 ( 板载 ) |
| 显示器   | PORPOISE 4K  |

---

### BIOS设置

1.Setting-高级-内建显示配置-集成显卡多显示器 [允许]  
2.Setting-高级-整合周边设备-网络协议栈       [允许]  
3.OC-扩展内存预设技术(XMP)                   [Enabled]  
4.OC-CPU Features-CFG Lock                   [Disabled]
> 懒得设置可以直接开启D.T.M设置（会关闭cnvi网卡，需要手动开启）
> 如果可以，建议把`Intel C-State`关闭，提高系统运行稳定性

---

### 完美程度
- 核显加速，显存1536MB；华擎5500XT ITX补全缓冲帧 显卡优化
- 睡眠正常，睡眠后，唤醒需要按一下开机键（BIOS可以设置开启PCI设备，USB设备唤醒）
- CPU 睿频正常
- 传感器正常工作、_CPU_ 温度、_SSD_ 温度风扇转速均可获取（通过iStat Menus查看）
- 定制主板后面USB映射正常
- 雷电三接口正常，由于没有笔者雷电设备，无法测试真正使用情况（有使用者跟我反馈，雷电3接口完美使用，包括外接触摸屏正常触摸使用）
- 核显硬解正常
- 单独使用核显情况下最多可以使用3块屏幕（DP、HDMI、雷电3）
- 有线网正常工作
- 蓝牙连接稳定，蓝牙音响、鼠标长时间正常工作
- 最新的intel网卡驱动，板载AX201上网已经完美使用了（好点Wi-Fi6路由链接速率可以达到1700Mbps+），接力功能正常，不支持隔空投放
- 蓝牙连接正常（蓝牙音响无噪音电流声），2.4G设备会有干扰，建议避开（master2s 如果用蓝牙连接稳定性会很好，不会干扰）
### FAQ
- 如果睡眠有问题，自己加个hibernate补丁驱动测试
- 如果使用核显，独显缓冲帧建议删除（不删除也不影响）。
- 默认配置config.plist定制端口（除了主板上拓展C口）
- 配置config-extend-typec.plist定制端口（除了主板上19pin，USB拓展），看自己喜好需要什么端口可以自行定制
- 替换EFI后在终端记得执行:`sudo kextcache -i/`
---
### IMAGES
<img src="/img/multi-core.png"/>
<img src="/img/iShot_2022-05-01_22.29.15.png"/>
<img src="/img/iShot2021-08-19 11.49.59.png"/>
<img src="/img/iShot_2022-05-01_22.16.37.png"/>
<img src="/img/iShot_2022-05-01_22.19.02.png"/>
<img src="/img/iShot_2022-05-01_22.19.51.png"/>
<img src="/img/7B4E3D81-0CE8-4BBD-A212-DE4E298646A1.png"/>
<img src="/img/031093CB-E667-4E95-A5B0-276124B1670C.png"/>
