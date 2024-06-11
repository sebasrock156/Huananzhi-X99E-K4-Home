[Aptio's V Tools ]: https://www.mediafire.com/file/ucvt4pdxjrtpmu7/Tools_for_AMI_Aptio_V.zip/file
[Aptio's Tools Mirror]: https://disk.yandex.com/d/XrZjsImaqxl8Uw
[Just right here]: https://github.com/sebasrock156/Huananzhi-X99E-K4-Opencore
[Audio Drivers]: https://www.mediafire.com/file/046t9639xeyr243/X99-P4FAudio.rar/file
[Ethernet Drivers for W10]: https://www.mediafire.com/file/z4w75jswapzof1j/X99-P4FLAN.rar/file
[Ethernet Drivers for W11]: https://www.mediafire.com/file/53yr2eb7w82h75v/X99-P4FLanwin11.zip/file
[Original BIOS Image]: https://www.mediafire.com/file/zozi3s0fixamce4/X99E-K4+BIOS.rom/file
[Unlocked BIOS Image]: https://www.mediafire.com/file/qtwh4jle25884rq/X99E-K4_VGXX02_Unlocked.rom/file
[Chipset Driver]: https://www.mediafire.com/file/kevqagczu5b4igy/X99-P4FChipset.rar/file
[AMI EXPRESS GUIDE]: https://github.com/sebasrock156/Huananzhi-X99E-K4-Home/blob/main/AMIXpress-Guide.md

# Huananzhi X99E-K4 Software Home

![Motherboard](https://i.imgur.com/FtSCjxq.png)

I will try to give some unofficial support for the cheapest Huananzhi Motherboard, using 3rd party programs and utilities for this end.

And yes, I want to correct the missing/erroneous data that Huananzhi has put on the specifications, so I put a new list with the same corrected ones

<details>
  
---
Component | Description
---|:--:
Chipset | Intel P55 or HM55 (randomly)
Socket  | Intel LGA 2011-3
RAM Memory Slots | DDR4(x4) until 128GB Support (Max.)
RAM Memory Freq. | Quad-channel (on 4 slots) support since 1866Mhz until 2400Mhz ECC or Non-ECC modules
Storage interface | Sata 2.0(x3)@3Gbps
Storage expansion | One slot M.2 2280 NVME PCIEx4 3.0@32Gbps or M.2 NGFF Sata 2.0@3Gbps
Audio card | Realtek HD Audio ALC897 (Surround 5.1 Support max.)
Network card | Realtek Ethernet RTL8168 1Gbps.
Power interface | ATX 24pin + ATX 12v 8pin
Fan interface | CPU Fan(x2) 4 pin (Fans with 3 pin connector are compatible too)
Power supply | Between 6 to 8 phases of power supply (600W PSU or better)
Dimensions | 210*182mm Micro-ATX
Rear panel | PS/2 Port(x2), USB 2.0@480Mbps(x6), Network port (RJ45), Audio interface (3 jacks)
Front panel | (Connectors only) USB 2.0(1x), USB 3.0(x1) Audio interface (x1) COM port (x1), Power/Reset interface
Supported system | Windows (7, 10 and 11), GNU/Linux (x86_64), MacOS (with Hackintosh only)
---
</details>

### Why do I contradict the manufacturer?

<details>
  
  ![specs](https://i.imgur.com/fAamx7u.png)

  Here is the prove of RAM configuration:

  - I'm using the 4 DIMM Slots with Corsair's ValueSelect 8GB(x4) modules.

  - When I used only 2 DIMM Slots, Windows detected the RAM configuration as Dual-Channel.

  ![prove1](https://i.imgur.com/y0NncYc.png)

  Some interesting thing about this motherboard is, their BIOS Settings, this is configured for a real X99 Chipset, so, if we use programs as HWInfo, we have things like this:

  ![interesting](https://i.imgur.com/BtQmmwF.png)

  
</details>

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

[Unlocked BIOS Image]: This is a BIOS image with Overclock Settings enabled/unlocked. (**THIS IS FOR XEON 16xx V3/V4 AND CORE EXTREME PROCESSORS ONLY; I CAN'T GUARANTEE GOOD RESULTS**)

Try use the Turbo Boost Hack if you have a Xeon V3; in my case, I have a Xeon V4 and may not work at all.

### Lightweight Overclock guide

1. Boot to BIOS Interface and go to **IntelRCSetup-->Advanced Power Manager Configuration-->CPU Advanced PM Tuning-->Program PPO_CURT_CFG_CTRL_MSR** and change:
   - **PPO Current_Cfg_CTL Ovrd** to **MANUAL**
   - **Current Config** option to **Enable**
   - **Current limitation** to **2048**
2. Now go back to main **IntelRCSetup** and later go to **Overclocking Feature**:

   *Overclocking Feature needs to be ENABLED for continue*

   Now go to **Processor** and change:
    - **Core Voltage Mode** to **Override**
    - **Core Voltage Override** to **XXXX**, where (XXXX) it's some Voltage multiple; If your processor have 90W or 105W of TDP usually, use 1.1v/1.2v for run with all their cores, so, with this option, we go to force a Voltage limit that processor can use in Motherboard, *eg: I have a Xeon E5-2640v4 that have 90W of TDP, I want define that MoBo force 1.2v for it, so, define the Core Voltage Override value as 1200*
  
3. Now exit to BIOS Interface with F4 and save the changes.


---

</details>

## BIOS Modifying Utilities

<details>
  
⚠ **ADVICE** ⚠: Here I want appeal at Fair Use, some tools are leaks from Technical Services and Enterprises, the Inverse Engineering of these are usually illegal, but here it's used for educational purposes.

[Aptio's V Tools] | [Aptio's Tools Mirror]: These tools are we could modify and flash new BIOS Firmwares.

To know how they work, I attach the [AMI EXPRESS GUIDE] to open and flash firmwares easily and simply.

---
</details>

## Manual/Assambly Guide

IN DEVELOPMENT, some previews below:

<details>
  
  ![GUIDE_MAIN](https://github.com/sebasrock156/Huananzhi-X99E-K4-Home/blob/main/Guide%20Project/UserGuideX99E-K4%20Coverlow.png?raw=true)
  ![GUIDE2](https://github.com/sebasrock156/Huananzhi-X99E-K4-Home/blob/main/Guide%20Project/Guide%20English/UserGuide2.png?raw=true)
  ![GUIDE3](https://github.com/sebasrock156/Huananzhi-X99E-K4-Home/blob/main/Guide%20Project/Guide%20English/UserGuide3.png?raw=true)

</details>

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
