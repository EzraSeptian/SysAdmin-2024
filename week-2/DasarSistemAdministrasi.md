---
marp: true
---

# **Dasar Sistem Administrasi**

    NRP   : 3122600016
    Nama  : Ezra Septian Handyanto
    Kelas : 2 D4 IT A
    Dosen : Dr. Ferry Astika Saputra, ST, M.Sc

---

# Discover: the KDE Package Manager

Gnome menggunakan software untuk me-manage aplikasi dengan cara sederhana, yaitu "Discover".

Discover dapat membantu kita untuk search, remove, atau update aplikasi kita dari satu interface. Kita juga dapat memodifikasi software source kita. (Secara mudah, Discover bekerja seperti Play Store)

Untuk membuka Discover, cukup masuk ke main menu > Application > System > Software Center > Discover

---

# Discovery Interface

![](../assets/week2-2.png)

![](../assets/week2-3.png)

![](../assets/week2-4.png)

---

# Discovery Interface

![](../assets/week2-5.png)

![](../assets/week2-6.png)

![](../assets/week2-7.png)

---

# Synaptic: the Comprehensive Package Manager

Synaptic adalah comprehensive graphical interface milik debian package manager

Ini memungkinkan untuk melihat total dari packages yang dipilih, baik terinstall maupun yang belum. Ini jauh lebih detail darpiada Discovery karena Synaptic menampilkan set lengkap packages yang tersedia. (termasuk libraries-nya)

---

# Synaptic Interface

![](../assets/week2-8.png)

![](../assets/week2-11.png)

---

# Synaptic Interface

![](../assets/week2-10.png)

![](../assets/week2-12.png)

---

# Synaptic Interface

![](../assets/week2-13.png)

![](../assets/week2-9.png)

---

# Cleaning the System

Sebelum ke bagian cleaning, terdapat beberapa tools untuk mengetahui ruang yang digunakan dalam disk.

Kita bisa menggunakan terminal dengan `df -h` atau Disk Usage Analytics, application langsung dari debian.

---

![](../assets/week2-15.png)

---

![](../assets/week2-16.png)

---

# Cleaning Procedures

Untuk membersihkan disk kita, kita akan memulai dari langkah pertama, yaitu:

## Cleaning the Packages :

using terminal

`apt clean`
`apt autoremove --purge`
`aot list ?obsolete`
`apt remove '?obsolete`

---

# Cleaning Procedures

## Emptying the Trash Bins :

using terminal

`rm -Rf ~/.local/share/Trash/*` > user wastebasket
`rm -Rf /root/.local/share/Trash/*` > admin wastebasket
`/media/your_id/your_disk/.Trash_1000` > external wastebasket

---

# Cleaning Procedures

## Purging Application Caches :

using terminal
`rm -Rm ~/.cache/*`

## Purging the thumbnails :

using terminals
`rm -Rf ~/.thumbnails`

---

# Paket .deb

deb adalah kependekan dari Debian. Untuk mendistribusikan softwarenya, Debian menggunakan format file arsip berupa .deb. .deb merupakan suatu format untuk mengkompres banyak file pada Debian seperti .zip pada Windows.

---

# Install di graphic mode dengan GDebi

GDebi merupakan graphical utility dimana dapat melakukan instalasi package dengan format .deb. Untuk install GDebi lakukan apt update && apt install gdebi menggunakan mode "su". Untuk menggunakan GDebi klik kanan pada file .deb lalu klik "Open with gdebi"

![](./assets/gdebi1.PNG)

---

Kemudian klik Install Package untuk menginstall Package.

![](/assets/gdebi2.PNG)

Lalu tunggu hingga proses selesai.

---

Untuk menghapus package klik Remove Package

![](/assets/gdebi3.PNG)

---

# Install di terminal menggunakan Dpkg

Untuk menginstall external package gunakan:

dpkg -i package_name.deb

Tetapi akan muncul pesan error dimana dependencies tidak tersedia. untuk mengatasinya lakukan:

apt install dependency_1 dependency_2 ... (sesuai kebutuhan)

kemudian lakukan ulang dpkg -i package_name.deb

dan untuk menghapusnya lakukan dpkg --purge package_name

---

# Flatpak

Flatpak adalah sistem aplikasi virtualisasi untuk distribusi GNU/Linux. Tujuannya adalah menyediakan lingkungan "sandbox" yang aman, terisolasi dari sistem utama, di mana pengguna dapat menjalankan aplikasi yang tidak divalidasi oleh repositori distribusi (misalnya, versi uji coba). Aplikasi yang diunduh dari repositori Debian adalah arsip berformat ".deb" yang berisi aplikasi itu sendiri. Aplikasi ini menggunakan dependensi umum, saling terhubung, dan memiliki akses ke seluruh sistem Anda. Repositori Debian aman, jadi tidak perlu khawatir tentang masalah ini. Namun, mengapa kita harus menggunakan Flatpak? Format Flatpak bekerja secara berbeda: aplikasi dikompresi bersama dengan semua dependensinya, menjadikannya sepenuhnya independen dari sistem di mana ia diinstal. Dengan demikian, di sini Anda dapat menginstal dan menggunakan aplikasi yang diperbarui secara segar atau bahkan yang baru, dibandingkan dengan repositori Debian.

---

# Install Flatpak

Untuk melakukan instalisasi Flatpak masukkan perintah

sudo apt install flatpak

---

# Menambahkan sebuah Repository Flatpak

Untuk menambahkan repository seperti flathub contohnya lakukan

flatpak remote-add flathub https://flathub.prg/repo/flathub.flatpakrepo

---

# Memanage aplikasi Flatpak menggunakan Gnom dengan Software

Untuk mengambil keuntungan dari managing flatpaks tanpa menggunakan software manager, kita harus menambahkan plugin yang sesuai dengan enviornment kita. Untuk Gnome kita dapat menginstallnya dengan perintah

sudo apt install gnome-software-plugin-flatpak

---

# Memanage aplikasi Flatpak menggunakan KDE dengan Discover

Untuk menggunakan KDE dalam hal memanage aplikasi Flatpak kita dapat menginstallnya menggunakan perintah

sudo apt install plasma-discover-backend-flatpak

---

# Memanage aplikasi Flatpak menggunakan terminal

List perintah:

flatpak search flaptak_name: untuk mencari sebuah flatpak di semua repositories

flatpak install repository flatpak_name: menginstall flatpak dari repository

flatpak uninstall flatpak_name: menghapus flatpak

flatpak uninstall -unused: menghapus dependencies yang tidak terpakai

flatpak update: melakukan update semua flatpak yang terinstall

flatpak run flatpak_name: menjalankan flatpak

---

# Siapa sid guy?

Secara singkat, Debian memiliki beberapa cabang distribusi yang berjalan sejajar, yaitu oldstable, stable, testing, dan unstable, serta cabang eksperimental. Distribusi Stable adalah distribusi resmi Debian yang dirilis pada saat ini, yang dipelihara dan diperbarui oleh tim Debian. Perubahan yang dilakukan hanya berkaitan dengan pembaruan keamanan dan perbaikan bug. Disarankan untuk menggunakan versi ini. Distribusi Oldstable adalah versi stabil sebelumnya yang biasanya didukung oleh tim Debian selama satu tahun setelah rilis versi stabil baru. Namun, bisa bertahan lebih lama jika cukup banyak individu atau perusahaan yang melanjutkan pemeliharaannya. Distribusi Testing adalah versi Stable masa depan yang digunakan untuk mempersiapkan versi stabil berikutnya. Distribusi Unstable, yang disebut Sid, adalah versi yang menerima semua versi paket baru dan berada di ujung inovasi, tetapi tidak sangat stabil. Ini adalah laboratorium penelitian. Distribusi Eksperimental bukanlah distribusi Debian yang sebenarnya, tetapi merupakan repositori di mana versi perangkat lunak alpha atau beta diuji.
