---
title: "Osu! Lazer Di Linux"
date: 2018-02-19T19:23:22+07:00
draft : false
tags : ["osu","linux"]
categories : ["linux","game"]
featureimage : "/img/osu!-lazer-di-linux/1.png"
menu : ""
description : ""
---
Sebenernya dah lama mau nyoba install [osu! lazer](https://blog.ppy.sh/) di linux cuman karena **_'katanya'_** osu lazer masih banyak _bug_ jadi males.Nah,kebetulan tadi temen ngirim screenshot dari osu lazer saya yang lagi enak-enak nonton <s>citrus</s> gintama langsung close dan cari-cari info soal osu lazer di linux (archlinux).
setelah beberapa jam nyoba-nyoba akhirnya terinstall juga , berikut screenshot osu lazer di archlinux saya.
<center>
![osu lazer di linux](/img/osu!-lazer-di-linux/4.png)
![osu lazer di linux](/img/osu!-lazer-di-linux/5.png)
![osu lazer di linux](/img/osu!-lazer-di-linux/8.png)
![osu lazer di linux](/img/osu!-lazer-di-linux/9.png)
![osu lazer di linux](/img/osu!-lazer-di-linux/10.png)
![osu lazer di linux](/img/osu!-lazer-di-linux/14.png)
![osu lazer di linux](/img/osu!-lazer-di-linux/17.png)
![osu lazer di linux](/img/osu!-lazer-di-linux/16.png)
</center>
## Install osu!lazer di linux
sebelum install osu lazer bagi kalian pengguna archlinux bisa ketik 'yaourt -S smbuild-bin' atau ubuntu 'sudo apt-get install smbuild'
oke langsung aja:
```bash
  1. git clone https://github.com/ppy/osu
  2. cd osu
  3. git submodule update --init --recursive
  4. wget https://dist.nuget.org/win-x86-commandline/latest/nuget.exe
  5. mono ./nuget.exe restore
  6. smbuild
  7. cd osu.Desktop/bin/Debug/
  8. mono 'osu!.exe'
```
## Warning!
osu!lazer masih memiliki bug jadi untuk kalian yang mau nyoba-nyoba silahkan install tapi jangan berharap lebih.
