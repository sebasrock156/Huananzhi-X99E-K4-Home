[Aptio's V Tools ]: https://www.mediafire.com/file/ucvt4pdxjrtpmu7/Tools_for_AMI_Aptio_V.zip/file
[Aptio's Tools Mirror]: https://disk.yandex.com/d/XrZjsImaqxl8Uw
[Just right here]: https://github.com/sebasrock156/Huananzhi-X99E-K4-Opencore
[Audio Drivers]: https://www.mediafire.com/file/046t9639xeyr243/X99-P4FAudio.rar/file
[Ethernet Drivers for W10]: https://www.mediafire.com/file/z4w75jswapzof1j/X99-P4FLAN.rar/file
[Ethernet Drivers for W11]: https://www.mediafire.com/file/53yr2eb7w82h75v/X99-P4FLanwin11.zip/file
[Original BIOS Image]: https://www.mediafire.com/file/zozi3s0fixamce4/X99E-K4+BIOS.rom/file
[Chipset Driver]: https://www.mediafire.com/file/kevqagczu5b4igy/X99-P4FChipset.rar/file

# Huananzhi X99E-K4 Software Home

![Motherboard](https://i.imgur.com/FtSCjxq.png)

I will try to give some unofficial support for the cheapest Huananzhi Motherboard, using 3rd party programs and utilities for this end.

## Drivers (Windows 10/11)

All the drivers below have been brought from other Huananzhi motherboars with similar or same components.

<details>

[Chipset Driver] (Inherited from X99-P4F Motherboard)

[Audio Drivers] (Inherited from X99-P4F Motherboard)

[Ethernet Drivers for W10] | [Ethernet Drivers for W11] (Inherited from X99-P4F Motherboard) 

⚠ **Disclaimer** ⚠: If you use utilities like Driver Booster, these drivers may corrupt things in the system, proceed with caution.

---
  
</details>

## BIOS Firmware

<details>
  
Since we haven't an official file from Huananzhi, I have taken the task of making a dump from my own Motherboard.

[Original BIOS Image]: This is a dump from Stock BIOS from my Motherboard, without modifies.

Try use the Turbo Boost Hack if you have a Xeon V3; in my case, I have a Xeon V4 and may not work at all.

---

</details>

## BIOS Modifying Utilities

<details>
  
⚠ **ADVICE** ⚠: Here I want appeal at Fair Use, some tools are leaks from Technical Services and Enterprises, the Inverse Engineering of these are usually illegal, but here it's used for educational purposes.

[Aptio's V Tools] | [Aptio's Tools Mirror]: These tools are we could modify and flash new BIOS Firmwares.

---
</details>

## Manual/Assambly Guide

IN DEVELOPMENT

## What CPU/Processor is supported?

<details>
Based on Socket (LGA 2011-3), all processors with that socket may be supported, but, the Southbridge (Chipset) is a mistery, I listed below some tested processors with this MoBo:

---
Series | Model | Specifications | Notes
---|---|---|:--:
Core | i7-5820K | Haswell-E, 6 Cores/12 Threads@3.3 GHz/3.6GHz Turbo, TDP 140W | Compatible with a 500W PSU  
Core | i7-5930K | Haswell-E, 6 Cores/12 Threads@3.5 GHz/3.7GHz Turbo, TDP 140W | Compatible with a 500W PSU
Core | i7-6800K | Broadwell-E, 6 Cores/12 Threads@3.4 GHz/3.6GHz Turbo, TDP 140W | Compatible with a 500W PSU
Core | i7-6850K | Broadwell-E, 6 Cores/12 Threads@3.6 GHz/3.8GHz Turbo, TDP 140W | Compatible with a 500W PSU
Core | i7-6900K | Broadwell-E, 8 Cores/16 Threads@3.2 GHz/3.7GHz Turbo, TDP 140W | Compatible with a 500W PSU
Core Extreme | i7-5960X | Haswell-E, 8 Cores/16 Threads@3.0 GHz/3.5GHz Turbo, TDP 140W | Compatible with a 500W PSU
Core Extreme | i7-6950X | Broadwell-E, 10 Cores/20 Threads@3.0 GHz/3.5GHz Turbo, TDP 140W | Compatible with a 650W PSU
Xeon | E5-1600 and E5-2600 V3 Series | Haswell-EP | Compatible with a 750W PSU or more
Xeon | E5-1600 and E5-2600 V4 Series | Broadwell-EP | Compatible with a 750W PSU or more
Xeon | E5-4600 V3 Series | Haswell-EP | Compatible with a 650W PSU, but using ECC RAM modules only (check the bandwidth before)
Xeon | E5-4600 V4 Series | Broadwell-EP | Compatible with a 750W PSU, but using ECC RAM modules only (check the bandwidth before)
---
  
</details>

## Can I do Hackintosh on it?

<details>

The short answer is YES, you can.

The long answer is YES, but: Really we are need to know what is the Motherboard Chipset (HM55 or P55), Audio Card and GPU that are using for run it.

For the variant with HM55 Chipset I'm working in some EFIes for boot MacOS as Hackintosh PC, [Just right here]

---
  
</details>

