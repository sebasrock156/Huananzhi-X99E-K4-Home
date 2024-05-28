[Herramientas para Aptio V]: https://www.mediafire.com/file/ucvt4pdxjrtpmu7/Tools_for_AMI_Aptio_V.zip/file
[Herramientas para Aptio V (Alt)]: https://disk.yandex.com/d/XrZjsImaqxl8Uw
[aquí mismo]: https://github.com/sebasrock156/Huananzhi-X99E-K4-Opencore
[Controlador de audio]: https://dlcdnets.asus.com/pub/ASUS/mb/01AUDIO/DRV_Audio_RTK_SZ_RTK_TSD_W10_64_V6090501_20210226R.zip?model=H81M-K
[Controlador de Red Ethernet]: https://dlcdnets.asus.com/pub/ASUS/lan/Realtek_LAN_Win7-8-81-10_V792115_838115_101505.zip?model=H81M-K

# Portal de Software de la Huananzhi X99E-K4

Intentaré brindar soporte no oficial para la placa base más barata de Huananzhi, utilizando programas y utilidades de terceros para este fin.

## Controladores/Drivers (Windows 10/11)

Todos los controladores a continuación fueron sugeridos por herramientas como Driver Booster.

<details>

[Controladores de Intel (Chipset, E/S y Procesador)]

[Controladores de la Placa Base (M.2, SATA, Puertos USB)]

[Controlador de Audio]: Éste está tomado de los oficiales de la H81M-K de Asus (que usa el Realtek ALC887 como dispositivo de audio)

[Controlador de Red Ethernet]: Éste está tomado de los oficiales de la H81M-K de Asus (Aunque realmente podrían ser de cualquier fabricante, el RTL8111/8160 es universal a día de hoy).

---
  
</details>

## Firmware de la BIOS

<details>
  
Como no tenemos un archivo oficial de Huananzhi, me he dado a la tarea de hacer un volcado desde mi propia placa base.

[Imagen de BIOS Original]: Esta es un volcado del BIOS de stock de mi placa base, sin modificaciones.

[Imagen de BIOS Desbloqueada]: Esta es una BIOS ligeramente modificada donde he intentado habilitar todo lo que está disponible.

[Imagen de BIOS Hackeada]: Esta es una imagen de BIOS modificada para los Xeon V3 (y algunos V4) con Turbo Boost Hack.

---

</details>

## Utilidades para modificación/flasheo de la BIOS

<details>
  
⚠ **Descargo de responsabilidad** ⚠: Aquí quiero apelar al Fair Use, algunas herramientas son filtraciones de Servicios Técnicos y Empresas, la Ingeniería Inversa de estas suele ser ilegal, pero aquí se usa con fines educativos.

[Herramientas para Aptio V] | [Herramientas para Aptio V (Alt)]: Estas herramientas nos permiten modificar y actualizar nuevos firmwares de la BIOS.

---
</details>

## Guía de ensamblaje/Manual

EN DESARROLLO

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

La respuesta larga es SI, pero: Realmente necesitamos saber cuál es el chipset de la placa base (HM55 o P55), la tarjeta de audio (normalmente la Realtek ALC887) y la GPU que se utilizará para inicializarlo (AMD o Nvidia, las discretas/dedicadas de Intel no tienen soporte).

Para la variante con chipset HM55 estoy trabajando en algunos EFI para arrancar MacOS como Hackintosh [aquí mismo]

---
  
</details>

