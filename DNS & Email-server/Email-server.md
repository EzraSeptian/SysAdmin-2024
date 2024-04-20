

`Tugas ini merupakan tugas mata kuliah Konsep Jaringan yang dibimbing oleh Bpk. Dr. Ferry Astika Saputra,ST, M.Sc`

## Table of Contents
- [NTP Client](#installing-ntp-client)
- [Apache-FM](#install-apache-fm)
- [PHP 8.2](#install-php-8.2)
- [MariaDB](#install-mariadb)
- [Email System](#email-system)
- [Dovecot Server](#install-dovecot-server)
- [Final Check](#last-check)





# Installing NTP Client

Lakukan instalasi paket layanan sinkronisasi waktu

![](asset/week5-1.PNG)

Pastikan konfigurasi timezone ke Asia/Jakarta

![](asset/week5-2.PNG)

Melakukan konfigurasi Real Time Clock (RTC) untuk merefer ke UTC (Coordinated Universal Time)


![](asset/week5-3.PNG)

Mengaktifkan NTP Client untuk sinkronisasi waktu

![](asset/week5-4.PNG)

Menyunting file timesyncd.conf untuk mengarah ke NTP server terdekat untuk mendapatkan waktu 
delay terpendek. Biasanya setiap organisasi atau negara mempunyai NTP Server sendiri

![](asset/week5-6.PNG)

![](asset/week5-5.PNG)

Restart layanan sinkronisasi waktu dan pastikan layanan berjalan dengan benar

![](asset/week5-7.PNG)


# Install Apache-FM

Installing Apache2

![](asset/week5-8.PNG)

Konfigurasi Apache2

`nano /etc/apache2/conf-enabled/security.conf`

`line 12 : change`

`ServerTokens Prod`

<br>

`nano vi /etc/apache2/mods-enabled/dir.conf`

`add file name that it can access only with directory's name`

`DirectoryIndex index.html index.htm`

<br>

`nano /etc/apache2/apache2.conf`

`line 70 : add to specify server name`

`ServerName www.kelompok3.com`

<br>

`nano /etc/apache2/sites-enabled/000-default.conf`

`line 11 : change to webmaster's email`

`ServerAdmin webmaster@kelompok3.com`

`systemctl reload apache2`

![](asset/week5-9.PNG)

Test ke web browser

![](asset/week5-10.PNG)


# Install PHP 8.2

![](asset/week5-11.PNG)

![](asset/week5-12.PNG)

![](asset/week5-13.PNG)

![](asset/phpinfo.PNG)

# Install PHP-FM

![](asset/week5-14.PNG)

![](asset/week5-15.PNG)

![](asset/week5-16.PNG)

# Install MariaDB

![](asset/week5-17.PNG)

![](asset/week5-18.PNG)

# Email System

![](asset/week5-19.PNG)

![](asset/week5-20.PNG)

![](asset/week5-21.PNG)

# Install Dovecot Server

![](asset/week5-22.PNG)

![](asset/week5-23.PNG)

## Last Check

![](asset/week5-24.PNG)

![](asset/week5-25.PNG)
