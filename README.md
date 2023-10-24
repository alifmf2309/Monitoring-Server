# Monitoring Server #
Tugas yang di buat pada final project kali ini adalah menginstall php monitoring server dengan php versi 7.4.
***

## Apa Itu PHP Monitoring Server? ##
PHP Monitoring Server adalah sebuah service yang memeriksa apakah situs web dan server Anda aktif dan berjalan. Dengan user interface berbasis web di mana Anda dapat mengelola layanan dan situs web Anda, dan Anda dapat mengelola pengguna untuk setiap server dengan nomor ponsel dan alamat email. Untuk contoh dari penggunaannya adalah sebagai berikut :

![image](https://github.com/alifmf2309/Monitoring-Server-menggunakan-PHP-Monitoring-Server/assets/117895406/def86bde-0e62-4af4-a40e-350384f2590e)

Ini adalah contoh ketika memonitoring sebuah website yaitu google.com. Demikian deskripsinya adalah sebagai berikut :

![image](https://github.com/alifmf2309/Monitoring-Server-menggunakan-PHP-Monitoring-Server/assets/117895406/6a8e9590-b4eb-4c2e-acc7-257b435cca29)
***

## OS Server ##
CentOS 7.9 64bit
***

## Repository Yang Digunakan ##
1. Local Repository (Insert DVD / CD CentOS-7-x86_64-DVD-2009.iso lalu di mount dan buat repository)
2. Cloud Repository (Menggunakan wget (link package yang akan di install)
3. Epel Repository (Extra Packages for Enterprise Linux. Di install servicenya dari repository online maupun offline)
***

## Bahan dan Alat ##
1. File ISO CentOS 7, dapat di download di http://isoredirect.centos.org/centos/7/isos/x86_64/
2. FTP Server menggunakan FileZilla untuk memudahkan manajemen file.
3. SSH Server untuk meremote server.
4. PHP 7.4 / diatasnya.
5. MySQL.
6. MariaDB.
7. PHP Server Monitor.
***

## Service Yang Digunakan ##
1. SSH Server
2. DHCP Server
3. Apache2
4. MariaDB
5. PHP Versi 7.4
6. FTP Server menggunakan FileZilla
***

## Update Progress ##
1. 17 September 2023 Instalasi SSH Server
2. 17 September 2023 Instalasi DHCP Server
3. 12 Oktober 2023  Instalasi Apache2 dan MariaDB
4. 14 Oktober 2023 Instalasi PHP Versi 7.4
5. 16 Oktober 2023 Instalasi FTP Server (Service pada CentOS dan software FileZilla pada Windows)
6. 20 - 21 Oktober 2023 Instalasi PHP Server Monitor versi v3.6.0
***

## Panduan Instalasi ##
Git adalah sistem kontrol versi terdistribusi yang melacak perubahan dalam setiap set file komputer, biasanya digunakan untuk mengoordinasikan pekerjaan di antara programmer yang secara kolaboratif mengembangkan kode sumber selama pengembangan perangkat lunak. Repositori Git menawarkan banyak layanan, salah satunya GitHub.

**Install Git terlebih dahulu**
```
[root@localhost ~]# yum install git
[root@localhost ~]# git clone https://github.com/phpservermon/phpservermon
[root@localhost ~]# cd phpservermon
[root@localhost phpservermon]#
```

Apabila sudah mendapatkan clone package PHP Server Monitor dari GitHub, masuk ke direktori <code>phpservermon</code> lalu install package <code>composer.phar</code>.

**Dilanjut untuk install php composer.phar**
```
[root@localhost phpservermon]# php composer.phar install
Loading composer repositories with package information
Installing dependencies (including require-dev) from lock file
Package operations: 19 installs, 0 updates, 0 removals
    Failed to download mnsami/composer-custom-directory-installer from dist: The zip extension and unzip command are both missing, skipping.
Your command-line PHP is using multiple ini files. Run `php --ini` to show them.
```


Apabila terdapat error <code>Failed, The zip extension and unzip command are both missing</code>, install dahulu package zip unzip dengan command <code>yum install zip unzip</code>.

**Install Zip Unzip dilanjut untuk install php composer.phar**
```
[root@localhost phpservermon]# yum install zip unzip
Installed:
  unzip.x86_64 0:6.0-24.el7_9                                                    zip.x86_64 0:3.0-11.el7

Complete!
[root@localhost phpservermon]# php composer.phar install
.
.
Generating autoload files
[root@localhost phpservermon]#
```
