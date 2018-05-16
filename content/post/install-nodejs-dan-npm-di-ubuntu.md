---
title: "Install Nodejs Dan Npm Di Ubuntu"
date: 2018-05-16T14:40:00+07:00
draft: false
thumbnail : "img/install-nodejs-npm-di-ubuntu-01.jpg"
---
{{% img src="img/nodejs-npm.jpg" w="600" h="400" class="left" %}}
Node.js adalah platform perangkat lunak pada sisi-server dan aplikasi jaringan. Ditulis dengan bahasa JavaScript dan dijalankan pada Windows, Mac OS X, dan Linux tanpa perubahan kode program. Node.js memiliki pustaka server HTTP sendiri sehingga memungkinkan untuk menjalankan server web tanpa menggunakan program server web seperti Apache atau Lighttpd.

npm adalah package manager untuk JavaScript.
{{% clear %}}
Untuk installasi nodejs dan npm di ubuntu pertama buka terminal kalian, setelah itu ketik
```
sudo apt install nodejs npm
```
setelah installasi selesai npm belum bisa di gunakan untuk menginstall package secara global dikarenakan tempat default npm untuk menyimpan package global itu milik root, sebenarnya bisa kalian akali dengan menambahkan `sudo`

```
sudo npm i -g nama_package
```
hanya saja cara ini tidak disarankan, caranya yang paling baik adalah dengan mengganti folder default npm tersebut berikut caranya:

#### 1.buat folder untuk npm modules package
```
mkdir ~/.node_modules
```
**node_modules** adalah nama folder untuk tempat package npm bisa kalian ubah terserah.

#### 2.jalankan ini diterminal untuk mengubah folder default package npm
```
NPM_CONFIG_PREFIX=~/.npm-global
```
[docs npm tentang masalah permission](https://docs.npmjs.com/getting-started/fixing-npm-permissions)

## source
+ [npm nodejs](https://id.wikipedia.org/wiki/Node.js)
+ [npm wikipedia](https://en.wikipedia.org/wiki/Npm_(software))