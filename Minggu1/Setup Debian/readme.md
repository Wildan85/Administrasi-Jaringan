
# SET UP DEBIAN

1. Siapkan Oracle VM VirtualBox, kemudian pilih 'New'
   
![](Assets/1.png)

2. Masukkan nama dan file iso debian di ISO Image
   
![Arsitektur Jaringan Kampus](2.png)

3. Atur Base Memory dan CPU yang dibutuhkan
   
![Arsitektur Jaringan Kampus](3.png)

4. Atur penyimpanan sesuai yang dibutuhkan
   
![Arsitektur Jaringan Kampus](4.png)

5. Summary berisi detail OS yang di atur sebelumnya, kemudian finish
    
![Arsitektur Jaringan Kampus](5.png)

6. Tampilan awal set debian, pilih bahasa yg akan digunakan
    
![Arsitektur Jaringan Kampus](6.png)

7. Pilih lokasi
    
![Arsitektur Jaringan Kampus](7.png)

![Arsitektur Jaringan Kampus](8.png)

8. Set keyboard
    
![Arsitektur Jaringan Kampus](9.png)

9. Masukkan hostname (SysAdmin-NRP)
    
![Arsitektur Jaringan Kampus](10.png)

10. Nama domain kosong/default
    
![Arsitektur Jaringan Kampus](11.png)

11. Masukkan password
    
![Arsitektur Jaringan Kampus](12.png)

12. Masukkan username
    
![Arsitektur Jaringan Kampus](13.png)

13. Atur waktu
    
![Arsitektur Jaringan Kampus](14.png)

14. Atur partisi hard disk, pilih manual
    
![Arsitektur Jaringan Kampus](15.png)

15. Set bagian vbox harddisk
    
![Arsitektur Jaringan Kampus](16.png)

16. Pilih Ya
    
![Arsitektur Jaringan Kampus](17.png)

17. Partisi yang selesai dibuat
    
![Arsitektur Jaringan Kampus](18.png)

18. Pilih kobo.pens.ac.id untuk mengatur pengelola paket
    
![Arsitektur Jaringan Kampus](19.png)

19. Kosongkan alamat http
    
![Arsitektur Jaringan Kampus](20.png)

20. Pasang boot loader GRUB dan pilih hardisk yang sebelumnya
    
![Arsitektur Jaringan Kampus](21.png)

21. Selesai Instalasi

![Arsitektur Jaringan Kampus](22.png)

22. Tampilan Debian
    
![Arsitektur Jaringan Kampus](23.png)

# Perbedaan Debian 12 (Bookworm) dan Debian 11 (Bullseye)

![Arsitektur Jaringan Kampus](24.png)

# Fungsi dari File "/etc/group" dan Formatnya
File "/etc/group" berisi informasi tentang grup-grup pengguna pada sistem. Setiap baris mewakili satu grup dan memiliki format sebagai berikut:

nama_grup:password:ID_grup:anggota1,anggota2,...

- nama_grup: Nama grup.
- password: Biasanya berisi "x", dan sebenarnya password grup disimpan di "/etc/gshadow".
- ID_grup: ID numerik unik untuk grup.

#  Perbedaan antara "su" dan "su -"

- su: Mengganti pengguna tanpa mengganti lingkungan shell. Variabel lingkungan, seperti PATH, tetap dari pengguna sebelumnya.
- su -: Mengganti pengguna dan juga mengganti ke lingkungan shell yang baru. Ini sama dengan login sebagai pengguna tersebut dan membawa seluruh lingkungan pengguna tersebut.

# Fungsi dari "sudo"

"sudo" (superuser do) adalah perintah yang memungkinkan pengguna untuk menjalankan perintah sebagai pengguna lain, biasanya sebagai superuser (root). Ini memberikan hak akses terbatas dan terkontrol kepada pengguna, yang dicatat dan dilacak.

#  Langkah-langkah penambahan user sebagai user sudo

- Gunakan perintah su - untuk masuk sebagai root.
- Setelah masuk sebagai root, jalankan perintah visudo untuk mengedit file konfigurasi sudoers.
- Tambahkan baris berikut di bawah baris yang mencakup user root pada bagian " # User privilege specification":
  * username ALL=(ALL:ALL) ALL
  * (Gantilah "username" dengan nama pengguna yang ingin User tambahkan.)
- Simpan dan keluar dari editor.

Dengan langkah-langkah ini, pengguna yang User tambahkan akan memiliki hak akses sudo di sistem. Pastikan untuk memberikan hak akses sudo hanya kepada pengguna yang membutuhkannya dan amankan konfigurasi sudoers dengan hati-hati.
