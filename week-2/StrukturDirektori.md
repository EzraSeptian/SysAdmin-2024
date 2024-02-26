# Struktur Direktori Linux


## Perkenalan 

Di Windows, untuk mengakses suatu direktori menggunakan 
D:\Folder\subfolder\file.txt

Di Linux, format untuk mengaksesnya
/Folder/subfolder/file.txt

Pada Linux kita menggunakan / sedangkan pada windows kita menggunakan \ untuk membuka suatu direktori dan di Linux foldernya merupakan case sensitive semisal

/Folder/subfolder/file.txt itu tidak sama dengan /folder/subfolder/file.txt


## Ringkasan Struktur Linux Direktori

Struktur Direktori pada Unix & Linux adalah satu dimana Struktur Direktori terletak pada Root. Maksudnya semua direktori disusun secara hierarki di bawah sistem folder Root ("/")


Struktur Direktori Linux menerapkan "Filesystem Hierarchy Structur" (FHS) yang dikembangkan oleh Free Standards Group meskipun sebagian besar distribusi terkadang cenderung menyimpang dari standar.

## Penjelasan Direktori Pada Linux

### "/" Root

Struktur Direktori dimulai dari Root "/" dan Root dibutuhkan sebagai akar dari direktori untuk semua direktori di Linux

### /boot

Direktori /boot berisi file Boot Lodaer termasuk Grub atau Lilo, the Kernel dan system.map config files.

### /sys

Direktori ini berisi the Kernel, Firmware dan file system

### /sbin 

Direktori berisi Sistem Biner dan tools Sistem Administrasi yang berguna untuk sistem operasi dan performa.

### /bin

Direktori berisi biner yang penting dan merupakan keperluan bagi user pada mode single user. Contoh, perintah cat,ls,cp etc.

### /lib

Direktori berisi file library untuk semua biner yang berada pada direktori /sbin & /bin

### /dev

Direktori berisi sistem file dan drivers yang penting

### /etc

/etc/directory berisi konfigurasi sistem file penting termasuk /etc/hosts, /etc/resolv.conf, nsswitch.conf default dan konfigurasi file network.
