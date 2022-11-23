---
layout: post
title: PulseAudio, menuju tak terbatas dan melampauinya
date: 2022-11-23 04:36:25 0500
categories: [Linux, Tutorial]
tags: [Linux, Audio, PulseAudio]
---

assalamualaikum kawan, jadi saya habis install ulang arch linux dan saat dengar lagu suaranya kok kecil?
jadi disini ada caranya mengatasi pulseaudio suaranya mentok di 100%.
oke, pertama kalian install 
`pulseaudio pulseaudiocontrol pulseaudio-equalizer`
dengan pacman atau apt atau dnf.
## pacman  (arch based)
```terminal
sudo pacman -S pulseaudio pulseaudiocontrol pulseaudio-equalizer
```
## apt-get  (debian based)
```terminal
sudo apt-get install pulseaudio pulseaudiocontrol pulseaudio-equalizer
```
> yg apt saya belum pernah coba, tapi anda coba saja :)
{: .prompt-info }
setelah itu kalian buat shortcut keyboard agar kalian nanti tdk ngetik perintah banyak2

pergi ke settingan keyboard dan tambahkan shortcut terserah kalian dan 
tambahkan
```
pactl -- set-sink-volume 0 +50%
```
sebagai perintah yg dijalankan.

dan selamat sekarang kalian sudah bisa atur volumenya sesuai keinginan kalian :).