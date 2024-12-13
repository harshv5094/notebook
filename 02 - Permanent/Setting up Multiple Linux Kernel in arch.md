---
tags:
  - linux
  - arch
Created on: 13-11-2024 18:11
URL: https://itsfoss.com/switch-kernels-arch-linux/
---
# How to setup multiple Linux kernel and add Grub menu option

## Step 1: Install Kernels

Just run this commands to install different kernels:

- For `latest`:

```bash
sudo pacman -S linux
```

- For `lts`:

```bash
sudo pacman -S linux-lts
```

## Step 2: Tweak the grub configuration file to add more kernel options

1. First edit `/etc/default/grub` file using your favorite editor:

```bash
sudo nvim /etc/default/grub
```

2. Add this line in the config, or modify if already present in the config.

```c
GRUB_DISABLE_SUBMENU=y
GRUB_DEFAULT=saved
GRUB_SAVEDEFAULT=true
```

## Step 3: Re-generate the GRUB configuration file

Run this b

```bash
sudo grub-mkconfig -o /boot/grub/grub.cfg
```
