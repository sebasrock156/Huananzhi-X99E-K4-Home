[Ferramentas pra Aptio V]: https://www.mediafire.com/file/ucvt4pdxjrtpmu7/Tools_for_AMI_Aptio_V.zip/file
[Ferramentas pra Aptio V (Alt)]: https://disk.yandex.com/d/XrZjsImaqxl8Uw
[aqui]: https://github.com/sebasrock156/Huananzhi-X99E-K4-Opencore
[Dirver de áudio]: https://www.mediafire.com/file/046t9639xeyr243/X99-P4FAudio.rar/file
[Driver de rede Ethernet pra W10]: https://www.mediafire.com/file/z4w75jswapzof1j/X99-P4FLAN.rar/file
[Driver de rede Ethernet pra W11]: https://www.mediafire.com/file/53yr2eb7w82h75v/X99-P4FLanwin11.zip/file
[Imagem original do BIOS]: https://www.mediafire.com/file/zozi3s0fixamce4/X99E-K4+BIOS.rom/file
[Imagem do BIOS desbloqueada]: https://www.mediafire.com/file/x4vfwu4vqol0hdd/X99E-K4+Unlocked.rom/file
[Driver de chipset]: https://www.mediafire.com/file/kevqagczu5b4igy/X99-P4FChipset.rar/file
[GUIA EXPRESS do AMI]: https://github.com/sebasrock156/Huananzhi-X99E-K4-Home/blob/main/AMIXpress-Guide.md

# Portal do Software pra Huananzhi X99E-K4

![Motherboard](https://i.imgur.com/FtSCjxq.png)

Tentarei fornecer suporte não oficial para a placa-mãe Huananzhi mais barata, usando programas e utilitários de terceiros para issa finalidade.

E sim, quero corrigir os dados ausentes/errôneos que Huananzhi colocou nas especificações, então colocarei uma lista atualizada

<details>
  
---
Componente | Descrição
---|:--:
Chipset | Intel P55 ou HM55 (aleatório)
Soquete | Intel LGA 2011-3
Slots de memória RAM | DDR4 (x4) com suporte até 128GB (máx.)
Frequência de RAM | Suporte a Quad-Channel (em 2 ou 4 slots) de 1866 MHz a 2400 MHz com módulos ECC ou non-ECC
Interface de armazenamento | Sata 2.0(x3)@3Gbps
Expansão de armazenamento | Um slot M.2 2280 NVME PCIEx4 3.0@32Gbps ou M.2 NGFF Sata 2.0@3Gbps
Placa de áudio | Realtek HD Audio ALC897 (suporta Surround 5.1 máx.)
Placa de rede | Realtek Ethernet RTL8168 1Gbps.
Interface de fluxo | ATX de 24 pinos + ATX de 8 pinos 12v
Interface de dissipação | Ventilador de CPU de 4 pinos (x2) (ventiladores com conector de 3 pinos também são compatíveis)
Fonte de alimentação | Entre 6 a 8 fases de alimentação (com fontes de 600W ou superior)
Dimensões | 210*182mm Micro-ATX
Painel traseiro | Porta PS/2 (x2), USB 2.0@480Mbps (x6), porta de rede (RJ45), interface de áudio (3 conectores)
Painel frontal | (Somente conectores) Interface de áudio USB 2.0(1x), USB 3.0(x1) (x1) Porta COM (x1), Interface liga/desliga - reiniciar
Sistema suportado | Windows (7, 10 e 11), GNU/Linux (x86_64), MacOS (somente com Hackintosh)
---
</details>


## Controladores/Drivers (Windows 10/11)

Todos os drivers abaixo foram retirados de outras placas-mãe Huananzhi com componentes iguais ou semelhantes.

<details>

[Driver de chipset] (Trouxe de X99-P4F)

[Dirver de áudio] (Trouxe de X99-P4F)

[Driver de rede Ethernet pra W10] | [Driver de rede Ethernet pra W11] (Trouxe de X99-P4F)


⚠ **Aviso Legal** ⚠: Se você usar utilitários como o Driver Booster, esses drivers podem corromper coisas no sistema, proceda com cuidado.

---
  
</details>

## Firmware do BIOS

<details>
  
Como não temos um arquivo oficial de Huananzhi, assumi a tarefa de fazer um dump da minha própria placa-mãe.

[Imagem original do BIOS]: Este é um dump do BIOS padrão da minha placa-mãe, sem modificações.

[Imagem do BIOS desbloqueada]: Este é um BIOS com configurações de Overclock habilitadas/desbloqueadas. (**RECOMENDADO SOMENTE PARA PROCESSADORES XEON 16XX V3/V4 E CORE EXTREME; TAMBÉM NÃO GARANTO BONS RESULTADOS**)

Experimente o Turbo Boost Hack se você tiver um Xeon V3; no meu caso, tenho um Xeon V4 e pode não funcionar.

---

</details>

## Utilitários de modificação/flash do BIOS

<details>
  
⚠ **Aviso Legal** ⚠: Aqui quero apelar ao Fair Use, algumas ferramentas são vazamentos de Serviços Técnicos e Empresas, a Engenharia Reversa destas geralmente é ilegal, mas aqui é usada para fins educacionais.

[Ferramentas pra Aptio V] | [Ferramentas pra Aptio V (Alt)]: Essas ferramentas nos permitem modificar e atualizar novos firmwares de BIOS.

Para saber como funcionam, anexei o [GUIA EXPRESS do AMI] (em inglês) para abrir e atualizar firmwares de forma fácil e simples.

---
</details>

## Guia/Manual de Montagem

EM DESENVOLVIMENTO, baseado nos originais de Huananzhi.

## Qual CPU/processador é compatível?

<details>
Baseado em Socket (LGA 2011-3), todos os processadores com esse soquete podem ser suportados, mas o Southbridge (Chipset) é um mistério. Abaixo listei alguns processadores testados com esta placa-mãe:
---
Série | Modelo | Especificações | Notas
---|---|---|:--:
Core | i7-5820K | Haswell-E, 6 núcleos/12 threads@3,3 GHz/3,6 GHz Turbo, TDP 140W | Compatível com fontes do 500W 
Core | i7-5930K | Haswell-E, 6 Núcleos/12 threads@3.5 GHz/3.7GHz Turbo, TDP 140W | Compatível com fontes do 500W 
Core | i7-6800K | Broadwell-E, 6 Núcleos/12 threads@3.4 GHz/3.6GHz Turbo, TDP 140W | Compatível com fontes do 500W 
Core | i7-6850K | Broadwell-E, 6 Núcleos/12 threads@3.6 GHz/3.8GHz Turbo, TDP 140W | Compatível com fontes do 500W 
Core | i7-6900K | Broadwell-E, 8 Núcleos/16 threads@3.2 GHz/3.7GHz Turbo, TDP 140W | Compatível com fontes do 500W 
Core Extreme | i7-5960X | Haswell-E, 8 Núcleos/16 threads@3.0 GHz/3.5GHz Turbo, TDP 140W | Compatível com fontes do 500W 
Core Extreme | i7-6950X | Broadwell-E, 10 Núcleos/20 threads@3.0 GHz/3.5GHz Turbo, TDP 140W | Compatível com fontes do 650W
Xeon | Série E5-16XX e E5-26XX V3 | Haswell-EP | Compatível com fontes do 750W ou mais
Xeon | Série E5-16XX e E5-26XX V4 | Broadwell-EP | Compatível com fontes do 750W ou mais
Xeon | Série E5-46XX V3 | Haswell-EP | Compatível com fontes do 750W ou mais, mas usando apenas módulos de RAM ECC (verifique a largura de banda primeiro)
Xeon | Série E5-46XX V4 | Broadwell-EP | Compatível com fontes do 1000W ou mais, mas usando apenas módulos de RAM ECC (verifique a largura de banda primeiro)
---
  
</details>
