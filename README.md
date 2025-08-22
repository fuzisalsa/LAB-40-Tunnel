# LAB-40-Tunnel
tanggal 22 agustus 2025

# tunnel 
IP tunnel adalah kanal jaringan komunikasi Protokol Internet (IP) antara dua jaringan komputer yang digunakan untuk transportasi menuju jaringan lain dengan mengkapsulkan paket ini. IP Tunnel sering kali digunakan untuk menghubungkan dua jaringan IP tidak bergabung yang tidak memiliki alamat penjaluran asli (native routing path) ke lainnya, melalui protokol penjaluran utama melewati jaringan transportasi tingkat menegah. Bersama dengan protokol IPsec keduanya kemungkinan digunakan untuk membuat jaringan maya pribadi (Virtual Private Network) antara dua atau lebih jaringan pribadi melewati jaringan umum misalnya internet.

# konfigurasi router bali 
1. lakukan konfigurasi dasar  
2. jika sudah terhubung ke internet kita pilih menu       
   interfaces > ip tunnel      
3. klik (+)  
4. masukkan nama (opsional)  
   lalu local address : ip publik bali   
   remote address : ip publik jawa   
   klik ok  

![m](j1.PNG)

5. jika muncul flag R maka artinya router bali dan jawa sudah terhubung

![m](j2.PNG)

6. lalu kita tambahkan ip address untuk interface ip tunnel bali-jawa    
   pilih menu ip > address   
   klik (+)   
   address : ip yang sudah di berikan router jawa 10.208.10.2  
   network : ip address router jawa 10.208.10.1   

![m](j3.PNG)

7. lalu coba ping ke router jawa

![m](j5.PNG)

8. lalu kita buatkan routing  
   pilih menu ip > routes   
   klik (+)   
   dst.address adalah ip lan dari router jawa  
   gateway : 10.208.10.1  

![m](j4.PNG)

9. kita coba tes di laptop lewat cmd bukti bahwa bisa berkomunikasi 

![m](j6.PNG)

# keimpulan

tunnel adalh Teknik yang  digunakan untuk menghubungkan dua jaringan secara aman atau virtual, terutama ketika kedua jaringan berada di lokasi yang berbeda secara geografis.

# sumber

https://youtu.be/icnJrQjiUW4?si=FUUvyRla8IwyFnva
