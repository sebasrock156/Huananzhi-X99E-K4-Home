[Aptio's V Tools]: https://www.mediafire.com/file/ucvt4pdxjrtpmu7/Tools_for_AMI_Aptio_V.zip/file
[Mirror]: https://disk.yandex.com/d/XrZjsImaqxl8Uw

# AMIBIOS Modifying Guide (The fastest way)

> ⚠ **DISCLAIMER** ⚠: This guide makes use of Fair Use to explain in an educational and didactic way how to reprogram a BIOS without using external hardware with official tools from the >manufacturer itself leaked on the internet.
>
>Reproduction, reverse engineering, commercialization or profiting from these tools in an unauthorized manner is completely illegal and penalized in different countries.
>
>The Original Poster (OP) is already taking a risk by sharing this method and these tools without the express permission of American Megatrends from this Github file.
>
>Obviously, the original poster is not responsible for the use/abuse of these tools by third parties, nor for thermonuclear explosions that occur on your motherboard if you make strange modifications to your BIOS.
>
>YOU HAVE BEEN WARNED!


Here I will explain in the briefly possible way how to modify an American Megatrends (AMI) BIOS, although each of these tools comes with a more extensive user guide for programmers and hardware manufacturers, you can refer to them at any time to try to modify your BIOS in depth.

So, download [Aptio's V Tools] | [Mirror] and extract it with any unzipper.


## 1. Introducing to the tools

<details>

Once unzipped, we will have the following files:
   
Aptio V AMI Firmware Update Utility (**AFU**): This is to safely dump and/or flash all of our BIOS images to the motherboard without using an external programmer.

This has 3 variants:
 
- AFUDOS: For flash BIOS firmwares from DOS System/Command Prompt or Legacy BIOSes

- AFUEFI: For flash BIOS firmwares from a USB Memory Stick on UEFI BIOSes (GNU/Linux OSes included). 

- AFUWIN: For flash BIOS firmwares from Windows 7/8/8.1/10 with some intuitive options (command prompt) or an understandable interface (GUI).


AMI BIOS Guard Firmware Update Tool (**AMIBGT**, within AFU files): This is a trusted BIOS Flasher for firmwares with Intel Bios Guard Security available.

This has 2 variants:

 - BGTEFI: For flash BIOS firmwares from a USB Memory Stick on UEFI BIOSes (GNU/Linux). 

 - BGTWIN: For flash BIOS firmwares from Windows 7/8/8.1/10 (command prompt)

AMI BIOS Configuration Program (**AMIBCP**): This is the cherry on the cake, where we can modify/unlock/hide parameters, settings, menus and anything else we can think of as long as the BIOS chip and the Chipset allow it. This is only available for Windows 7 and 10; on Windows 8/8.1 may be works but crash randomly.

---

</details>

## 2. Dumping your BIOS

<details>

Now, we proceed to execute AFU (in my case, AFUWINGUI):


![AFU1](https://i.imgur.com/yNsa8RU.png)

*Here we can see relevant information about the BIOS that is currently installed on our motherboard, such as: The Operating System, the BIOS firmware size, the NVRAM size, the firmware version and GUID, and the chip model that our BIOS uses*.



In this specific case, I show how to make a dump of our already installed BIOS pressing the "Save" option:


![AFU2](https://i.imgur.com/Ca2yiq1.png)

*You can rename the dump file to the path and name you want as long as you don't change its .fd/.rom format*


When the dump process starts, it will automatically take you to the "Progress" tab.
While the dump process is running, you will not be able to use your computer until it is finished.

Once the process is complete, the "Progress" tab will look like this:

![AFU3](https://i.imgur.com/OA9pWGx.png)

*If «Stage» is "done" you could close the AFU program.*

---

</details>

## 3. Modifying the BIOS Firmware

<details>

Now that we have a dump of our BIOS firmware, we proceed to run AMIBCP to modify it.

*We go to the "Open 📂" option, look for our firmware in .fd/.rom format and select it*

![BCP1](https://i.imgur.com/gqltUUE.png)


At this point, we will see on the left panel, the entire structure of the firmware; while on the right side, each and every one of the options to customize are displayed.


![BCP2](https://i.imgur.com/uf588We.png)

*In this case, I will do the demonstration with the Overclocking settings*


As we can see, some specific values ​​can be defined such as:

- Control group structures: Also known as categories, this is where different sets of instructions are grouped together.
- Show: As the name suggests, it defines whether a category/instruction is visible (or not) in the BIOS Firmware.
- Access/Use: Defines who is the viewer of the categories/options in the BIOS interface. This is divided into 4 groups:

  - Default: Sets to a specific viewer type defined by the manufacturer (in this case AMI).
  - User: Defines any type of user that enters the interface as an observer.
  - Extended User: It is very similar to the previous one, but this observer can only access with certain "administrative permissions" (such as a password in the BIOS Firmware)
  - Supervisor: This observer needs to enable the BIOS "Administrator Mode" to see the categories/options
 
- Fail-safe: Defines specific parameters to be met, such as a switch, a data swap option or a toggle option (eg. Graphic memory allocation is the Category, User is the Access (viewer) on BIOS UI and "2GB" is the Fail-safe option, like a testing value). 
- Optimal: It is a parameter similar to the fail-safe parameter, but within values ​​previously established by the manufacturer (eg. Graphic memory allocation is the Category, User is the Access (viewer) on BIOS UI, "2GB" is the Fail-safe option and "128MB" is the Optimal option, like a final/effective value).


*Once our modification is complete, we can save (or save as) our modified firmware as seen below.*

![BCP3](https://i.imgur.com/ctFVcvQ.png)
  
</details>

# 4. Flashing a new BIOS firmware


