---
title: "Mengatur Active Area Wacom Di Linux"
date: 2018-02-25T07:12:12+07:00
draft : false
tags : ["linux","archlinux","wacom"]
categories : ["utility"]
featureimage : "/img/mengatur-active-area-wacom-di-linux/1.png"
menu : ""
description : ""
---
Jadi tadi malem habis dapet wacom dari seseorang.
![wacom](/img/mengatur-active-area-wacom-di-linux/1.png)  
Langsung saya pakek buat main osu dan entah kenapa kerasa kurang enak saya pun berfikir mungkin karena saya main di full active area setelah nyarik cara mengatur active area wacom di archlinux,akhirnya ketemu juga caranya:
![wacom di linux](/img/mengatur-active-area-wacom-di-linux/2.png)  
ketik `xsetwacom --list devices` untuk melihat list wacom device yang connect dengan pc/laptop mu
![wacom di linux](/img/mengatur-active-area-wacom-di-linux/3.png)  
ketik `xsetwacom --get " [nama] " Area` untuk melihat berapa size active area wacom kalian.
Sekarang tinggal kalian ingin berapa size active area katakanlah kalian punya active area `14720 x 9200` berarti kalau kalian ingin menjadikan active area 1/4 dari size awal tinggal bagi `14720 x 9200` dengan 4.
ketiakan `xsetwacom --set " [nama] " Area 0 0 [ukuran yang baru]`
![wacom di linux](/img/mengatur-active-area-wacom-di-linux/5.png)
saya sih menggunakan 1/4 dari size saya yang berarti saya menggunakan `0 0 3680 517`.Oke cukup sekian semoga bermanfaat.