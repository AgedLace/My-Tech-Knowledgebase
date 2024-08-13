---
title: Maintenance Commands
slug: maintenance
date: 2024-08-03 04:07:05
update: 2024-08-11 07:29:45
publish: "true"
tags:
  - Linux/ArchLinux/Commands/Maintenance
categories: 
---

## Check Systemd Failed Services

- `systemctl --failed`

## Log Files Check

- `sudo journalctl -p 3 -xb`

## Update

- `sudo pacman -Syu`

## Yay Update

- `yay`

## Delete Pacman Cache

- `sudo pacman -Sc`

## Delete Yay Cache

- `yay -Sc`

## Delete Unwanted Dependencies

- `yay -Yc`

## Check Orphan Packages

- `pacman -Qtdq`

## Remove Orphan Packages

- `sudo pacman -Rns $(pacman -Qtdq)`

## Clean the Cache

- `rm -rf .cache/*`

## Clean the Journal

-`sudo journalctl --vacuum-time=2weeks`
