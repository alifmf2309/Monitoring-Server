# Monitoring Server

## Tentang Tugas
Tugas yang di buat pada final project kali ini adalah menginstall php monitoring server dengan php versi 7.4.

## Apa Itu PHP Monitoring Server?
PHP Monitoring Server adalah sebuah service yang memeriksa apakah situs web dan server Anda aktif dan berjalan. Dengan user interface berbasis web di mana Anda dapat mengelola layanan dan situs web Anda, dan Anda dapat mengelola pengguna untuk setiap server dengan nomor ponsel dan alamat email. Untuk contoh dari penggunaannya adalah sebagai berikut :

![image](https://github.com/alifmf2309/Monitoring-Server-menggunakan-PHP-Monitoring-Server/assets/117895406/def86bde-0e62-4af4-a40e-350384f2590e)

Ini adalah contoh ketika memonitoring sebuah website yaitu google.com. Demikian deskripsinya adalah sebagai berikut :
![image](https://github.com/alifmf2309/Monitoring-Server-menggunakan-PHP-Monitoring-Server/assets/117895406/6a8e9590-b4eb-4c2e-acc7-257b435cca29)


## OS Server
CentOS 7.9 64bit

## Repository Yang Digunakan
1. Local Repository (Insert DVD / CD CentOS-7-x86_64-DVD-2009.iso lalu di mount dan buat repository)
2. Cloud Repository (Menggunakan wget (link package yang akan di install)
3. Epel Repository (Extra Packages for Enterprise Linux. Di install servicenya dari repository online maupun offline)

## Bahan dan Alat
1. File ISO CentOS 7, dapat di download di http://isoredirect.centos.org/centos/7/isos/x86_64/
2. FTP Server menggunakan FileZilla untuk memudahkan manajemen file.
3. SSH Server untuk meremote server.
4. PHP 7.4 / diatasnya.
5. MySQL.
6. MariaDB.
7. PHP Server Monitor.

## Service Yang Digunakan
1. SSH Server
2. DHCP Server
3. Apache2
4. MariaDB
5. PHP Versi 7.4
6. FTP Server menggunakan FileZilla

## Update Progress
1. 17 September 2023 Instalasi SSH Server
2. 17 September 2023 Instalasi DHCP Server
3. 12 Oktober 2023  Instalasi Apache2 dan MariaDB
4. 14 Oktober 2023 Instalasi PHP Versi 7.4
5. 16 Oktober 2023 Instalasi FTP Server (Service pada CentOS dan software FileZilla pada Windows)
6. 20 - 21 Oktober 2023 Instalasi PHP Server Monitor versi v3.6.0

## Panduan Instalasi
<code>
[root@localhost~]# yum install git
[root@localhost~]# git clone https://github.com/phpservermon/phpservermon
</code>
