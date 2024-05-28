[Aptio 的 V 工具]: https://www.mediafire.com/file/ucvt4pdxjrtpmu7/Tools_for_AMI_Aptio_V.zip/file
[Aptio的工具镜像]: https://disk.yandex.com/d/XrZjsImaqxl8Uw
[就在这里]: https://github.com/sebasrock156/Huananzhi-X99E-K4-Opencore
[音频驱动程序]: https://dlcdnets.asus.com/pub/ASUS/mb/01AUDIO/DRV_Audio_RTK_SZ_RTK_TSD_W10_64_V6090501_20210226R.zip?model=H81M-K
[适用于 W10 的以太网驱动程序]: https://www.mediafire.com/file/z4w75jswapzof1j/X99-P4FLAN.rar/file
[适用于 W11 的以太网驱动程序]: https://www.mediafire.com/file/53yr2eb7w82h75v/X99-P4FLanwin11.zip/file
[原始 BIOS 映像]: https://www.mediafire.com/file/zozi3s0fixamce4/X99E-K4+BIOS.rom/file
[芯片组驱动程序]: https://www.mediafire.com/file/kevqagczu5b4igy/X99-P4FChipset.rar/file

# 华南X99E-K4软件主页

我将尝试为最便宜的华南智主板提供一些非官方支持，为此使用第 3 方程序和实用程序。

## 驱动程序 (Windows 10/11)

以下所有驱动程序均来自具有相似或相同组件的其他华南主板。

<details>

[芯片组驱动程序]（继承自 X99-P4F 主板）

[音频驱动程序]

[适用于 W10 的以太网驱动程序] | [适用于 W11 的以太网驱动程序] （继承自 X99-P4F 主板）


⚠ **免责声明** ⚠：如果您使用 Driver Booster 之类的实用程序，这些驱动程序可能会损坏系统中的某些内容，请谨慎操作。

---
  
</details>

## BIOS固件

<details>
  
由于我们没有华南志的正式文件，所以我承担了从我自己的主板上转储的任务。

[原始 BIOS 映像]：这是我主板上的 Stock BIOS 的转储，未经修改。

[解锁 BIOS 映像]：当我尝试启用其中的所有功能时，这是一个经过轻微修改的 BIOS。

[被黑的 BIOS 映像]：这是经过修改的 BIOS 映像，用于通过 Turbo Boost Hack 启动 Xeon V3 系列（和某些 V4 系列）。
---

</details>

## BIOS 修改实用程序

<details>
  
⚠ **免责声明** ⚠：在这里我想对合理使用提出上诉，有些工具是技术服务和企业泄露的，这些工具的逆向工程通常是非法的，但在这里它用于教育目的。

[Aptio 的 V 工具] | [Aptio的工具镜像]: 这些工具是我们可以修改和刷新新的 BIOS 固件的工具。

---
</details>

## 手册/组装指南

开发中

## 支持什么 CPU/处理器？

<details>

基于Socket（LGA 2011-3），所有具有该插槽的处理器都可能受支持，但是，南桥（芯片组）是一个谜，下面我列出了一些使用该主板测试的处理器：

---
系列 | 模型 | 规格 | 笔记
---|---|---|:--:
核心| i7-5820K | Haswell-E，6 核/12 线程@3.3 GHz/3.6GHz Turbo，TDP 140W |兼容500W电源 
核心| i7-5930K | Haswell-E，6 核/12 线程@3.5 GHz/3.7GHz Turbo，TDP 140W |兼容500W电源
核心| i7-6800K | Broadwell-E，6 核/12 线程@3.4 GHz/3.6GHz Turbo，TDP 140W |兼容500W电源
核心| i7-6850K | Broadwell-E，6 核/12 线程@3.6 GHz/3.8GHz Turbo，TDP 140W |兼容500W电源
核心| i7-6900K | Broadwell-E，8 核/16 线程@3.2 GHz/3.7GHz Turbo，TDP 140W |兼容500W电源
核心至尊| i7-5960X | Haswell-E，8 核/16 线程@3.0 GHz/3.5GHz Turbo，TDP 140W |兼容500W电源
核心至尊| i7-6950X | Broadwell-E，10 核/20 线程@3.0 GHz/3.5GHz Turbo，TDP 140W |兼容650W电源
至强 | E5-1600 和 E5-2600 V3 系列 | Haswell-EP |兼容 750W 或更高功率的 PSU
至强 | E5-1600 和 E5-2600 V4 系列 | Broadwell-EP |兼容 750W 或更高功率的 PSU
至强 | E5-4600 V3系列| Haswell-EP |兼容650W PSU，但仅使用ECC RAM模块（之前检查带宽）
至强 | E5-4600 V4系列| Broadwell-EP |兼容750W PSU，但仅使用ECC RAM模块（之前检查带宽）
---
  
</details>

## 我可以对它进行 Hackintosh 吗？

<details>

简短的回答是肯定的，可以。

长的答案是肯定的，但是：我们确实需要知道用于运行它的主板芯片组（HM55 或 P55）、声卡和 GPU 是什么。

对于带有 HM55 芯片组的变体，我正在一些 EFI 中工作，以将 MacOS 作为 Hackintosh PC 启动 [就在这里]

---
  
</details>

