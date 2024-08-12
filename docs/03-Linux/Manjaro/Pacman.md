---
title: Pacman
slug: pacman
date: 2024-08-03 04:07:05
update: 2024-08-11 07:31:22
publish: "true"
tags:
  - Linux/Manjaro/Pacman
categories: 
---
## Pacman

### How Do I Reinstall All Packages, Retaining Information on whether Something Was Explicitly Installed or as a Dependency?

To reinstall all the native packages: `pacman -Qnq | pacman -S -` or `pacman -S $(pacman -Qnq)` (the `-S` option preserves the installation reason by default).

You will then need to reinstall all the foreign packages, which can be listed with `pacman -Qmq`.

---

 SOURCE - [pacman - ArchWiki](https://wiki.archlinux.org/title/pacman#Manually_reinstalling_pacman)

 
---

### Foreign Packages to Reinstall

brave-beta-bin  
caprine  
gtkhash  
gtkhash-thunar  
logseq-desktop-bin  
manjaro-hotfixes  
pdfstudioviewer  
protonmail-bridge-bin  
protonmail-desktop
