[Outils pour Aptio V]: https://www.mediafire.com/file/ucvt4pdxjrtpmu7/Tools_for_AMI_Aptio_V.zip/file
[Outils pour Aptio V (Alt)]: https://disk.yandex.com/d/XrZjsImaqxl8Uw
[ici]: https://github.com/sebasrock156/Huananzhi-X99E-K4-Opencore
[Pilote du audio]: https://www.mediafire.com/file/046t9639xeyr243/X99-P4FAudio.rar/file
[Pilote réseau Ethernet pour W10]: https://www.mediafire.com/file/z4w75jswapzof1j/X99-P4FLAN.rar/file
[Pilote réseau Ethernet pour W11]: https://www.mediafire.com/file/53yr2eb7w82h75v/X99-P4FLanwin11.zip/file
[Image originale du BIOS]: https://www.mediafire.com/file/zozi3s0fixamce4/X99E-K4+BIOS.rom/file
[Pilote du chipset]: https://www.mediafire.com/file/kevqagczu5b4igy/X99-P4FChipset.rar/file

# Portail logiciel pour Huananzhi X99E-K4

![Motherboard](https://i.imgur.com/FtSCjxq.png)

J'essaierai de fournir un support non officiel pour la carte mère Huananzhi la moins chère, en utilisant des programmes et des utilitaires tiers à cet effet.

Et oui, je veux corriger les données manquantes/erronées que Huananzhi a mises dans les spécifications, je vais donc mettre en place une liste mise à jour.

<details>
  
---
Composant | Description
---|:--:
Chipset | Intel P55 ou HM55 (aléatoire)
Prise | Intel LGA2011-3
Emplacements de mémoire RAM | DDR4(x4) avec prise en charge jusqu'à 128Go (Max.)
Fréquence de la RAM. | Prise en charge de Quad-channel (en 2 ou 4 emplacements) de 1866 MHz à 2400 MHz avec modules ECC ou non-ECC
Interface de stockage | SATA 2.0(x3) à 3 Gbit/s
Extension du stockage | Un emplacement M.2 2280 NVME PCIEx4 3.0 à 32 Gbit/s ou M.2 NGFF Sata 2.0 à 3 Gbit/s
Carte audio | Realtek HD Audio ALC897 (prend en charge Surround 5.1 max.)
Carte réseau | Realtek Ethernet RTL8168 1 Gbit/s.
Interface de flux | ATX 24 broches + ATX 8 broches 12v
Interface de dissipation | Ventilateur CPU 4 broches (x2) (les ventilateurs avec connecteur 3 broches sont également compatibles)
Alimentation | Entre 6 et 8 phases d'alimentation (Avec sources de 600 W ou plus)
Dimensions | Micro-ATX 210*182 mm
Panneau arrière | Port PS/2 (x2), USB 2.0 à 480 Mbps (x6), port réseau (RJ45), interface audio (3 connecteurs)
Panneau avant | (Connecteurs uniquement) USB 2.0 (1x), interface audio USB 3.0 (x1) (x1) Port COM (x1), interface marche/arrêt - redémarrage
Système pris en charge | Windows (7, 10 et 11), GNU/Linux (x86_64), MacOS (uniquement avec Hackintosh)
---
</details>


## Contrôleurs/pilotes (Windows 10/11)

Tous les pilotes ci-dessous proviennent d'autres cartes mères Huananzhi avec des composants identiques ou similaires.

<details>

[Pilote du chipset] (extrait du X99-P4F)

[Pilote du audio] (extrait du X99-P4F)

[Pilote réseau Ethernet pour W10] | [Pilote réseau Ethernet pour W11] (extrait du X99-P4F)


⚠ **Avertissement** ⚠ : Si vous utilisez des utilitaires comme Driver Booster, ces pilotes peuvent corrompre des éléments du système, procédez avec prudence.

---
  
</details>

## Micrologiciel du BIOS

<details>
  
Comme nous n'avons pas de fichier officiel de Huananzhi, j'ai pris la tâche de faire un dump de ma propre carte mère.

[Image originale du BIOS] : Il s'agit d'un dump du BIOS d'origine de ma carte mère, sans modifications.

Essayez le Turbo Boost Hack si vous possédez un Xeon V3 ; dans mon cas, j'ai un Xeon V4 et ça risque de ne pas fonctionner du tout.

---

</details>

## Utilitaires pour modifier/flasher le BIOS

<details>
  
⚠ **Avertissement** ⚠ : Ici, je veux faire appel au Fair Use, certains outils sont des fuites de services techniques et d'entreprises, l'ingénierie inverse de ceux-ci est généralement illégale, mais ici, ils sont utilisés à des fins éducatives.

[Outils pour Aptio V] | [Outils pour Aptio V (Alt)]: Ces outils nous permettent de modifier et de mettre à jour les nouveaux firmwares du BIOS.

---
</details>

## Guide/Manuel d'assemblage

EN COURS DE DÉVELOPPEMENT, basé sur les originaux Huananzhi.

## Quel CPU/processeur est pris en charge ?

<details>
Basé sur Socket (LGA 2011-3), tous les processeurs dotés de ce socket peuvent être pris en charge, mais le Southbridge (Chipset) est un mystère. Ci-dessous, j'ai répertorié quelques processeurs testés avec cette carte mère:

---
Série | Modèle | Spécifications | Notes
---|---|---|:--:
Core | i7-5820K | Haswell-E, 6 cœurs/12 threads à 3,3 GHz/3,6 GHz Turbo, TDP 140 W | Compatible avec les sources de 500W  
Core | i7-5930K | Haswell-E, 6 cœurs/12 threads à 3.5 GHz/3.7GHz Turbo, TDP 140W | Compatible avec les sources de 500W
Core | i7-6800K | Broadwell-E, 6 cœurs/12 threads à 3.4 GHz/3.6GHz Turbo, TDP 140W | Compatible avec les sources de 500W
Core | i7-6850K | Broadwell-E, 6 cœurs/12 threads à 3.6 GHz/3.8GHz Turbo, TDP 140W | Compatible avec les sources de 500W
Core | i7-6900K | Broadwell-E, 8 cœurs/16 threads à 3.2 GHz/3.7GHz Turbo, TDP 140W | Compatible avec les sources de 500W
Core Extreme | i7-5960X | Haswell-E, 8 cœurs/16 threads à 3.0 GHz/3.5GHz Turbo, TDP 140W | Compatible avec les sources de 500W
Core Extreme | i7-6950X | Broadwell-E, 10 cœurs/20 threads à 3.0 GHz/3.5GHz Turbo, TDP 140W | Compatible avec les sources de 650W
Xeon | Séries E5-16XX et E5-26XX V3 | Haswell-EP | Compatible avec les sources de 750W ou plus
Xeon | Séries E5-16XX et E5-26XX V4 | Broadwell-EP | Compatible avec les sources de 750W ou plus
Xeon | Série E5-46XX V3 | Haswell-EP | Compatible avec les sources de 750W ou plus, mais en utilisant uniquement des modules RAM ECC (vérifiez d'abord la bande passante)
Xeon | Série E5-46XX V4 | Broadwell-EP | Compatible avec les sources de 750W ou plus, mais en utilisant uniquement des modules RAM ECC (vérifiez d'abord la bande passante)
---
  
</details>

## Puis-je faire du Hackintosh dessus?

<details>

La réponse courte est OUI, oui, vous le pouvez.

La réponse longue est OUI, mais : nous avons vraiment besoin de savoir quel est le chipset de la carte mère (HM55 ou P55), la carte audio (généralement la Realtek ALC897) et le GPU qui sera utilisé pour l'initialiser (AMD ou Nvidia, le processeur discret). ceux / dédiés d'Intel ne sont pas pris en charge).

Pour la variante du chipset HM55, je travaille sur certains EFI pour démarrer MacOS comme Hackintosh [ici]

---
  
</details>

