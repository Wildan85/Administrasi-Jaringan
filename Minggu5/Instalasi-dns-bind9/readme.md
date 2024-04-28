# SETUP DNS SERVER

* Langkah 1: Instalansi BIND9

1. Buka terminal
2. Update paket sistem:
![Arsitektur Jaringan Kampus](1.png)

![Arsitektur Jaringan Kampus](2.png)

3. install BIND9

![Arsitektur Jaringan Kampus](3.png)

* Langkah 2: Konfigurasi BIND9

1. Edit file /etc/bind/named.conf :

![Arsitektur Jaringan Kampus](4.png)

![Arsitektur Jaringan Kampus](5.png)

2. Edit file /etc/bind/named.conf.options :

![Arsitektur Jaringan Kampus](6.png)

![Arsitektur Jaringan Kampus](7.png)

![Arsitektur Jaringan Kampus](8.png)

3. Edit file /etc/bind/named.conf.local :

![Arsitektur Jaringan Kampus](9.png)

![Arsitektur Jaringan Kampus](10.png)

4. Edit file /var/lib/bind/db.kelompok9.local :

![Arsitektur Jaringan Kampus](11.png)

![Arsitektur Jaringan Kampus](12.png)

5. Edit file /var/lib/bind/db.kelompok9.local.inv :

![Arsitektur Jaringan Kampus](13.png)

![Arsitektur Jaringan Kampus](14.png)

6. Edit file /etc/resolv.conf :

![Arsitektur Jaringan Kampus](15.png)

![Arsitektur Jaringan Kampus](16.png)

* Langkah 4: Periksa Konfigurasi dan Restart BIND9

1. Periksa kesalahan konfigurasi:

![Arsitektur Jaringan Kampus](17.png)

![Arsitektur Jaringan Kampus](18.png)

![Arsitektur Jaringan Kampus](19.png)

2. Restart BIND9:

![Arsitektur Jaringan Kampus](20.png)

3. Periksa status BIND9 untuk memastikan tidak ada kesalahan:

![Arsitektur Jaringan Kampus](21.png)

4. Uji setup DNS

![Arsitektur Jaringan Kampus](22.png)

![Arsitektur Jaringan Kampus](23.png)