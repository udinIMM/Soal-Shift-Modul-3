# SOAL SHIFT MODUL 3
## PERATURAN
1. Waktu pengerjaan dari soal keluar, hingga hari Sabtu tanggal 11 April 2018 pukul 22.00 WIB.<br>
2. **TIDAK DIPERBOLEHKAN BERTANYA KONFIGURASI KEPADA ASISTEN**. Jadikan google sebagai teman kalian.<br>
2. Jika tidak ada pemberitahuan revisi soal dari asisten, berarti semua soal **BERSIFAT BENAR** dan **DAPAT DIKERJAKAN**.<br>
3. Default memory 96M kecuali memory untuk GUBENG, KUPANG & WIYUNG sebesar 128M.<br>
4. Tidak Diperkenankan menambah memory tanpa persetujuan asisten, resiko tanggung sendiri akibatnya.<br>
5. Gunakan IP yang sudah diberikan kepada masing-masing kelompok untuk IP DMZ dan IP TUNTAPnya.<br>
6. Plotting Asisten untuk demo dan revisi akan keluar pada hari Rabu, 11 April 2018.<br>
7. **Sebelum mengerjakan soal shift kali ini, silahkan hapus semua file UML Anda yang sudah dibuat sebelumnya.**<br>
(Jika Anda tetap memakai UML yang sudah ada, resiko ditanggung sendiri).<br>

## SOAL
Dongeng Jarkom 2018 bagian 2<br>
<p>2 tahun setelah Nanda jatuh hati kepada Ridho, PT. Cinta Abadi Jaya menjadi salah satu perusahaan terbesar di negaranya. Namun menurut Nanda yang selaku CEO dari perusahaan tersebut, infrastruktur jaringannya perlu dibangun ulang. Sebagai seorang pria, Ridho pun ingin menunjukkan kesetiaannya terhadap Nanda dan membantunya. Namun dimulai dari topologi jaringan yang sederhana dulu, seperti topologi berikut :</p>

![Topologi](/images/001.PNG)<br>

<p><b>GUBENG</b> sebagai router, <b>KUPANG</b> sebagai proxy server, <b>WIYUNG</b> sebagai DNS server, dan UML lainnya sebagai client. Awalnya mereka mengkonfigurasi IP pada setiap perangkat yang terdapat pada perusahaan PT. Cinta Abadi Jaya dengan ketentuan sebagai berikut : </p>

1. (1)Konfigurasi **subnet 1** dengan range 192.168.0.2 s.d. 192.168.0.100 dengan netmask 255.255.255.0<br>
2. (2)Konfigurasi **subnet 2** dengan range 192.168.1.101 s.d. 192.168.1.105 **DAN** 192.168.1.201 s.d. 192.168.1.205 dengan netmask 255.255.255.0<br>
3. (3)Konfigurasi agar **JAGIR** selalu mendapatkan IP 192.168.0.88 **TANPA** melakukan konfigurasi IP statis.<br>
4. (4)Konfigurasi agar **PAKIS** selalu mendapatkan IP 192.168.1.204 **TANPA** melakukan konfigurasi IP statis.<br>
5. (5)Konfigurasi agar **subnet 1** dan **subnet 2** mendapatkan konfigurasi DNS 202.46.129.2 dan 10.151.36.7<br>

<p>Setelah mengamati kinerja karyawan-karyawan barunya, ternyata ada saja karyawan yang terlalu asik internetan sehingga lupa waktu. Ridho dan Nanda membuat kebijakan baru untuk membatasi akses internet para karyawannya dengan cara membangun sebuah proxy server. Dengan pembatasan akses proxy seperti berikut :</p>

1. (6)Komputer - komputer yang terdapat pada **subnet 1** tidak dapat mengakses internet pada pukul **18.00 - 02.00 (esok harinya)**.<br>
2. (7)Komputer - komputer yang terdapat pada **subnet 2** hanya bisa mengakses internet dengan kecepatan akses 16 KBps pada hari **Senin - Jumat** pukul **18.00 - 02.00 (esok harinya)**.<br>

<p>Nanda merasa tidak nyaman dengan <i>search engine</i> yang bernama duckduckgo, karena dia merasa terlalu membingungkan jika harus mencari sesuatu disana. Ridho pun peka terhadap perasaan Nanda. (8)Akhirnya Ridho pun mengatur kalau ada karyawan yang mengakses halaman duckduckgo.com, akan langsung mengarah ke halaman google.com.</p>

<p>Satu bulan berlalu, ternyata tagihan <i>bandwidth</i> internet dari perusahaan PT. Cinta Abadi Jaya semakin membengkak. Untung saja Ridho pernah mengambil mata kuliah forensik digital semasa kuliahnya dan menemukan penyebab masalah yang berasal dari divisi riset. Kebetulan perusahaan tersebut bermitra dengan Informatika ITS yang sebagai divisi riset. IP milik divisi riset berada pada subnet <b>10.151.252.0/22</b> (Informatics_Wifi, Netmask 255.255.252.0). (9)Ridho ingin membatasi <i>bandwidth</i> seluruh komputer pada divisi tersebut sebesar 512 kbps dan (10)tidak bisa mengakses <b>fk.unair.ac.id dan mb.its.ac.id</b> setiap hari <b>Sabtu - Minggu</b> pukul <b>07.00 - 18.00</b> karena menyebabkan polusi pandangan. Setelah Ridho membuat kebijakan tersebut, dia juga tidak ingin segala aktifitas yang dilakukan oleh divisi riset diketahui publik. (11)Maka Ridho pun juga membuat sebuah konfigurasi agar semua yang berusaha mengakses 10.151.36.5 dengan port 5000 akan diblokir, karena halaman tersebut milik divisi riset.</p>

<p>(12)Kesokan harinya, Ridho pun mempunyai ide untuk mengatur proxy servernya kembali supaya mudah digunakan dan cukup ketik <b>proxy.caj.xxx.corp</b> dengan port <b>8080</b>. Setelah itu, Ridho juga mengatur agar siapapun yang menggunakan proxy perusahaan tersebut untuk login terlebih dahulu. (13)Akun yang digunakan untuk login ke proxy tersebut diatur Ridho sebagai berikut :</p>
- Username : karyawan[xxx]proxy<br>
- Password : karyawan[xxx]proxy<br>

## KETERANGAN
- **xxx** adalah nama kelompok masing-masing. Misal : **a01**.
- Disarankan menginstall **lynx** atau **links** pada **subnet 1** dan **subnet 2** untuk uji coba mengakses web.

### Sekian cerita dongeng Jarkom 2018 dan selamat mengerjakan