## i7 10700 + MSI-Z490I-Unify 核显 独显 Hackintosh EFI

- 当前支持 ~~ BigSur 11.5.1(经测试可以使用Catalina，但需要自行更换网卡驱动等等)  & Monterey 12.0b4


---


### 电脑配置

| 规格     | 详细信息                                     |
| -------- | ---------------------------------------- |
| 机箱 | FormD-T1             |
| 电源 | 银欣SX700-G             |
| CPU散热 | EK240             |
| 主板型号 | MSI-Z490I-Unify             |
| 处理器   | Intel Core i7 10700           |
| 内存     | Asgard 32GB 2x16GB DDR4 2666Mhz                 |
| 硬盘     | WDS500G3X0C-00SJG0 512GB M.2 NVMe                  |
| 显卡 | ASRock Radeon RX 5500 XT Challenger ITX 8G 1717MHz 8GHz GDDR6                            |
| 声卡     | Realtek ALCS1220A (Layout 7)                    |
| 板载网卡 | 英特尔® Wi-Fi 6 AX201 ( 板载 ) |
| 显示器   | Q2490W1  |

---

### BIOS设置

1.Setting\高级\内建显示配置\集成显卡多显示器 [允许]  
2.Setting\高级\整合周边设备\网络协议栈       [允许]  
3.OC\扩展内存预设技术(XMP)                   [Enabled]  
4.OC\CPU Features\CFG Lock                   [Disabled]  


---

### 完美程度
- 核显加速，显存1536MB；华擎5500XT ITX补全缓冲帧 显卡优化
- 睡眠正常
- _CPU_ 睿频正常，单核4.8，全核4.6
- 传感器正常工作、_CPU_ 温度、_SSD_ 温度风扇转速均可获取（通过iStat Menus查看）
- 定制USB映射正常
- 雷电三接口正常，由于没有笔者雷电设备，无法测试真正使用情况
- 有线网正常工作
- 更新了最新的intel网卡驱动，AX201已经完美使用了（笔者使用垃圾天线速率达到1000+Mbps
- 4k@60显示器输出正常，内建识别，亮度及音量可通过 _MonitorControl_ 控制

---

### 鸣谢
https://github.com/2742280997/z490i-unify  
https://github.com/kingwood77/MSI-Z490i-Unify-Hackintosh  
https://github.com/milkpeanut/MSI-Z490I-UNIFY-Hackintosh  
https://github.com/kreactnative/EFI-z490-ace-10700k-bigSur  

https://github.com/acidanthera/OpenCorePkg  
https://gitee.com/btwise/OpenCore_NO_ACPI  

https://github.com/OpenIntelWireless/itlwm  
https://github.com/OpenIntelWireless/HeliPort  
https://github.com/wjz304/Hackintosh-EFI-MSI-Z490i-Unify
