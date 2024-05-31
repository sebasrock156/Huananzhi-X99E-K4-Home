[Herramientas para Aptio V]: https://www.mediafire.com/file/ucvt4pdxjrtpmu7/Tools_for_AMI_Aptio_V.zip/file
[Herramientas para Aptio V (Alt)]: https://disk.yandex.com/d/XrZjsImaqxl8Uw
[aquí mismo]: https://github.com/sebasrock156/Huananzhi-X99E-K4-Opencore
[Controlador de audio]: https://www.mediafire.com/file/046t9639xeyr243/X99-P4FAudio.rar/file
[Controlador de Red Ethernet para W10]: https://www.mediafire.com/file/z4w75jswapzof1j/X99-P4FLAN.rar/file
[Controlador de Red Ethernet para W11]: https://www.mediafire.com/file/53yr2eb7w82h75v/X99-P4FLanwin11.zip/file
[Imagen de BIOS Original]: https://www.mediafire.com/file/zozi3s0fixamce4/X99E-K4+BIOS.rom/file
[Imagen de BIOS Desbloqueada]: https://www.mediafire.com/file/x4vfwu4vqol0hdd/X99E-K4+Unlocked.rom/file
[Controlador del Chipset]: https://www.mediafire.com/file/kevqagczu5b4igy/X99-P4FChipset.rar/file
[GUIA EXPRESS de AMI]: https://github.com/sebasrock156/Huananzhi-X99E-K4-Home/blob/main/AMIxpressguide.md

# Portal de Software de la Huananzhi X99E-K4

![Motherboard](https://i.imgur.com/FtSCjxq.png)

Intentaré brindar soporte no oficial para la placa base más barata de Huananzhi, utilizando programas y utilidades de terceros para este fin.

Y sí, quiero corregir los datos perdidos/erronéos que Huananzhi puso en las especificaciones, así que pondré una lista actualizada

<details>
  
---
Componente | Descripción
---|:--:
Chipset | Intel P55 o HM55 (al azar)
Zócalo  | Intel LGA 2011-3
Ranuras de memoria RAM | DDR4(x4) con soporte hasta 128GB (Max.)
Frecuencia de RAM. | Soporte Quad-channel (en 2 o 4 ranuras) desde 1866Mhz hasta 2400Mhz con modulos ECC o No-ECC
Interfaz de almacenamiento | Sata 2.0(x3)@3Gbps
Expansión de almacenamiento | Una ranura M.2 2280 NVME PCIEx4 3.0@32Gbps o M.2 NGFF Sata 2.0@3Gbps
Tarjeta de audio | Realtek HD Audio ALC897 (Soporta Surround 5.1 max.)
Tarjeta de red | Realtek Ethernet RTL8168 1Gbps.
Interfaz de corriente | ATX de 24 pines + ATX 12v de 8 pines
Interfaz de disipación | Ventilador para CPU(x2) de 4 pines (Ventiladores con conector de 3 pines también son compatibles)
Alimentación de energía | Entre 6 a 8 fases de alimentación (Con fuentes de 600W o superior)
Dimensiones | 210*182mm Micro-ATX
Panel trasero | PS/2 Port(x2), USB 2.0@480Mbps(x6), puerto de red (RJ45), interfaz de audio (3 conectores)
Panel frontal | (Solo conectores) USB 2.0(1x), USB 3.0(x1) interfaz de audio (x1) puerto COM (x1), Interfaz de encendido/apagado - reinicio
Sistema soportado | Windows (7, 10 y 11), GNU/Linux (x86_64), MacOS (solamente con Hackintosh)
---
</details>


## Controladores/Drivers (Windows 10/11)

Todos los controladores que estarán a continuación, se han tomado de otras placas base de Huananzhi con componentes iguales o similares.

<details>

[Controlador del Chipset] (Tomado de la X99-P4F)

[Controlador de Audio] (Tomado de la X99-P4F)

[Controlador de Red Ethernet para W10] | [Controlador de Red Ethernet para W11] (Tomado de la X99-P4F)


⚠ **Descargo de responsabilidad** ⚠: Si usas utilidades como Driver Booster, puede que dichos controladores corrompan cosas en el sistema, procede con precaución.

---
  
</details>

## Firmware de la BIOS

<details>
  
Como no tenemos un archivo oficial de Huananzhi, me he dado a la tarea de hacer un volcado desde mi propia placa base.

[Imagen de BIOS Original]: Esta es un volcado del BIOS de stock de mi placa base, sin modificaciones.

[Imagen de BIOS Desbloqueada]: Esta es una BIOS con los ajustes de Overclock habilitados/desbloqueados. (**RECOMENDADO ÚNICAMENTE PARA PROCESADORES XEON 16XX V3/V4 Y CORE EXTREME; TAMPOCO GARANTIZO BUENOS RESULTADOS**)

Intente realizar el Hack del Turbo Boost si tiene un Xeon V3; en mi caso, tengo un Xeon V4 y puede que no funcione en lo absoluto.

---

</details>

## Utilidades para modificación/flasheo de la BIOS

<details>
  
⚠ **Descargo de responsabilidad** ⚠: Aquí quiero apelar al Fair Use, algunas herramientas son filtraciones de Servicios Técnicos y Empresas, la Ingeniería Inversa de estas suele ser ilegal, pero aquí se usa con fines educativos.

[Herramientas para Aptio V] | [Herramientas para Aptio V (Alt)]: Estas herramientas nos permiten modificar y actualizar nuevos firmwares de la BIOS.

Para saber cómo funcionan, anexo la [GUIA EXPRESS de AMI] (en Inglés) para abrir y flashear firmwares de forma fácil y sencilla.

---
</details>

## Guía de ensamblaje/Manual

EN DESARROLLO, basado en los originales de Huananzhi.

## ¿Qué CPU/Procesador es soportado?

<details>
Basado en Socket (LGA 2011-3), todos los procesadores con ese socket pueden ser compatibles, pero el Southbridge (Chipset) es un misterio. A continuación enumeré algunos procesadores probados con esta Placa Base:

---
Serie | Modelo | Especificaciones | Notas
---|---|---|:--:
Core | i7-5820K | Haswell-E, 6 Núcleos/12 Hilos@3.3 GHz/3.6GHz Turbo, TDP 140W | Compatible con fuentes de 500W  
Core | i7-5930K | Haswell-E, 6 Núcleos/12 Hilos@3.5 GHz/3.7GHz Turbo, TDP 140W | Compatible con fuentes de 500W
Core | i7-6800K | Broadwell-E, 6 Núcleos/12 Hilos@3.4 GHz/3.6GHz Turbo, TDP 140W | Compatible con fuentes de 500W
Core | i7-6850K | Broadwell-E, 6 Núcleos/12 Hilos@3.6 GHz/3.8GHz Turbo, TDP 140W | Compatible con fuentes de 500W
Core | i7-6900K | Broadwell-E, 8 Núcleos/16 Hilos@3.2 GHz/3.7GHz Turbo, TDP 140W | Compatible con fuentes de 500W
Core Extreme | i7-5960X | Haswell-E, 8 Núcleos/16 Hilos@3.0 GHz/3.5GHz Turbo, TDP 140W | Compatible con fuentes de 500W
Core Extreme | i7-6950X | Broadwell-E, 10 Núcleos/20 Hilos@3.0 GHz/3.5GHz Turbo, TDP 140W | Compatible con fuentes de 650W
Xeon | Series E5-16XX y E5-26XX V3 | Haswell-EP | Compatible con fuentes de 750W o más
Xeon | Series E5-16XX y E5-26XX V4 | Broadwell-EP | Compatible con fuentes de 750W o más
Xeon | Serie E5-46XX V3 | Haswell-EP | Compatible con fuentes de 750W o más, pero usando solo módulos de RAM ECC (compruebe antes el ancho de banda)
Xeon | Serie E5-46XX V4 | Broadwell-EP | Compatible con fuentes de 1000W o más, pero usando solo módulos de RAM ECC (compruebe antes el ancho de banda)
---
  
</details>

## ¿Puedo hacer Hackintosh en ella?

<details>

La respuesta corta es SI, si que puedes.

La respuesta larga es SI, pero: Realmente necesitamos saber cuál es el chipset de la placa base (HM55 o P55), la tarjeta de audio (normalmente la Realtek ALC897) y la GPU que se utilizará para inicializarlo (AMD o Nvidia, las discretas/dedicadas de Intel no tienen soporte).

Para la variante con chipset HM55 estoy trabajando en algunos EFI para arrancar MacOS como Hackintosh [aquí mismo]

---
  
</details>

