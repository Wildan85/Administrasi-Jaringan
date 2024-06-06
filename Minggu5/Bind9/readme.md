# SETUP DNS SERVER

* Langkah 1: Instalansi BIND9

1. Buka terminal
2. Update paket sistem:
   
![](Assets/1.png)

![](Assets/2.png)

3. install BIND9

![](Assets/3.png)

* Langkah 2: Konfigurasi BIND9

1. Edit file /etc/bind/named.conf :

![](Assets/4.png)

![](Assets/5.png)

2. Edit file /etc/bind/named.conf.options :

![](Assets/6.png)

![](Assets/7.png)

![](Assets/8.png)

3. Edit file /etc/bind/named.conf.local :

![](Assets/9.png)

![](Assets/10.png)

4. Edit file /var/lib/bind/db.kelompok9.local :

![](Assets/11.png)

![](Assets/12.png)

5. Edit file /var/lib/bind/db.kelompok9.local.inv :

![](Assets/13.png)

![](Assets/14.png)

6. Edit file /etc/resolv.conf :

![](Assets/15.png)

![](Assets/16.png)

* Langkah 4: Periksa Konfigurasi dan Restart BIND9

1. Periksa kesalahan konfigurasi:

![](Assets/17.png)

![](Assets/18.png)

![](Assets/19.png)

2. Restart BIND9:

![](Assets/20.png)

3. Periksa status BIND9 untuk memastikan tidak ada kesalahan:

![](Assets/21.png)

4. Uji setup DNS

![](Assets/22.png)

![](Assets/23.png)
