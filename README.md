[![OpenCore](https://img.shields.io/badge/OpenCore-0.7.1-yellowgreen)](https://github.com/zf1976/MSI-MEG-Z490I-Unify-Hackintosh-OC-EFI/releases/tag/OC-0.7.1)
[![macOS](https://img.shields.io/badge/macOS-11.5.2-orange)](https://www.apple.com/macos/catalina/)
[![MODEL](https://img.shields.io/badge/Model-Z490I-blue)](https://tw.msi.com/Motherboard/MEG-Z490I-UNIFY/)
[![BIOS](https://img.shields.io/badge/BIOS-7C77v19-brightgreen)](#)


## i9 10850K + MSI-MEG-Z490I-Unify 核显 独显 Hackintosh EFI

- 当前支持 -- Monterey 12.1(可以使用Catalina、BigSur，但需要自行更换网卡驱动等等)


---


### 电脑配置

| 规格     | 详细信息                                     |
| -------- | ---------------------------------------- |
| 机箱 | Acat Xpro             |
| 电源 | 银欣SX700-G             |
| CPU散热 | EK240             |
| 主板型号 | MSI-Z490I-Unify             |
| 处理器   | Intel Core i9 10850K       |
| 内存     | Asgard 32GB 2x16GB DDR4 2666Mhz                 |
| 硬盘     | WDS500G3X0C-00SJG0 512GB M.2 NVMe                  |
| 显卡 | ASRock Radeon RX 5500 XT Challenger ITX 8G 1717MHz 8GHz GDDR6                            |
| 板载网卡 | 英特尔® Wi-Fi 6 AX201 ( 板载 ) |
| 显示器   | Q2490W1  |

---

### BIOS设置

1.Setting\高级\内建显示配置\集成显卡多显示器 [允许]  
2.Setting\高级\整合周边设备\网络协议栈       [允许]  
3.OC\扩展内存预设技术(XMP)                   [Enabled]  
4.OC\CPU Features\CFG Lock                   [Disabled]  
> 懒得设置可以直接开启D.T.M设置（会关闭cnvi网卡，需要手动开启）


---

### 完美程度
- 核显加速，显存1536MB；华擎5500XT ITX补全缓冲帧 显卡优化
- 睡眠正常
- 睡眠后，唤醒需要按一下开机键，不能鼠标跟键盘唤醒，应该是没开启原生电源管理问题（BIOS可以设置开启PCI设备，USB设备唤醒）
- _CPU_ 睿频正常
- 传感器正常工作、_CPU_ 温度、_SSD_ 温度风扇转速均可获取（通过iStat Menus查看）
- 定制USB映射正常
- 雷电三接口正常，由于没有笔者雷电设备，无法测试真正使用情况（有使用者跟我反馈，雷电3接口完美使用，包括外接触摸屏正常触摸使用）
- 核显硬解正常
- 单独使用核显情况下最多可以使用3块屏幕（DP、HDMI、雷电3）
- 有线网正常工作
- 更新了最新的intel网卡驱动，板载AX201已经完美使用了（笔者使用垃圾天线速率达到1000+Mbps
### FAQ
- 如果使用核显，独显缓冲帧建议删除。
- 替换EFI后在终端记得执行:`sudo kextcache -i/`
---
### IMAGES
<img src="/images/neofetch.png"/>
<img src="/images/wifi.jpg"/>
<img src="images/iShot2021-08-19 11.49.59.png"/>
