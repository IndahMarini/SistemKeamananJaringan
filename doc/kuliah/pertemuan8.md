RESUME PERTEMUAN 8 KEAMANAN JARINGAN

TUTORIAL INSTALL SNORT Di centOS

1.Latar Belakang

Untuk mensupport suatu sitem dibutuhkan suatu distribusi contohnya Centos untuk mendukung proyek independen. Centos adalah distribusi Linux yang mencoba untuk memberikan gratis kelas enterprice, komunitas yang didukung platform komputasi fungsional kompatibel dengan sumber hulu , Red Hat Enterprice Linux (RHEL).

2. Pengertian

Centos adalah distribusi Linux yang mencoba untuk memberikan gratis kelas enterprice, komunitas yang didukung platform komputasi fungsional kompatibel dengan sumber hulu , Red Hat Enterprice Linux (RHEL).

Snort adalah salah satu yang paling umum digunakan untuk IDS berbasis jaringan. Ini adalah sistem open source yang tersedia untuk banyak platform , ringan dan dapat nyaman diinstall bahkan di terkecil dari contoh server cloud

Untuk mempersiapkan server maka harus menyiapkan konfigurasi snort dasar yang cukup sederhana  . kita harus menginstal semua perangkat lunak prasyarat untuk siap cloud  server  untuk menginstall snort sendiri dengan perintah berikut

Sudo yum install gcc flex bison zlib libpcap pcre libdnet libdnet-devel tcpdump.

3. Instalasi dengan yum

Snort memberikan paket rpm nyaman untuk CentOS 7, yang dapat diinstal hanya dengan perintah di bawah ini. Snort sendiri menggunakan sesuatu yang disebut Data Acquisition perpustakaan (DAQ) untuk melakukan panggilan abstrak untuk packet capture perpustakaan. Periksa nomor versi terbaru dari website Snort, jika versi yang lebih baru dari DAQ atau Snort tersedia cukup mengganti nomor versi di perintah berikut dengan opsi terbaru.

4. Instalasi dari source

Menyiapkan Snort dari kode sumber terdiri dari beberapa langkah: download kode, mengkonfigurasi, kompilasi kode dan terakhir menginstal itu. Pertama membuat folder download sementara untuk direktori home Anda dan kemudian bergerak ke dalamnya dengan perintah ini

mkdir ~/snort\_src

cd ~/snort\_src

Download paket terbaru sumber DAQ dari website Snort dengan perintah wget bawah, ganti nomor versi jika ada sumber yang lebih baru yang tersedia

wget https://www.snort.org/downloads/snort/daq-2.0.6.tar.gz

Download hanya akan memakan waktu beberapa detik, ekstrak setelah selesai kode sumber dan melompat ke dalam direktori baru dengan perintah berikut

tar -xvzf daq-2.0.6.tar.gz

cd daq-2.0.6

Jalankan script konfigurasi dengan default, kemudian gunakan membuat untuk mengkompilasi program dan kemudian akhirnya memasang DAQ

./configure

make

sudo make install

Dengan DAQ yang diinstal Anda bisa memulai dengan Snort, mengubah kembali ke folder download

cd ~/snort\_src

Kemudian download kode sumber Snort dengan wget, memeriksa nomor versi terbaru dari situs Snort dan menggantinya di perintah berikut jika diperlukan.

wget https://www.snort.org/downloads/snort/snort-2.9.8.0.tar.gz

Setelah download selesai, ekstrak sumber dan mengubah ke dalam direktori baru dengan perintah ini

tar -xvzf snort-2.9.8.0.tar.gz

cd snort-2.9.8.0

Kemudian mengkonfigurasi instalasi dengan modus Sourcefire diaktifkan, jalankan make dan make install.

./configure --enable-sourcefire

make

sudo make install

5. Penutup

Kesimpulan

 Centos adalah distribusi Linux yang mencoba untuk memberikan gratis kelas enterprice, komunitas yang didukung platform komputasi fungsional kompatibel dengan sumber hulu , Red Hat Enterprice Linux (RHEL).

Saran

        Agar pembaca mencari referensi lainnya untuk menambah pengetahuan tentang cara menginstall snort di centos.

NAMA        : INDAH MARINI RIZKY SIHOMBNG

NPM                : 1144041

KELAS        : 3C

PRODI        : D4 TEKNIK INFORMATIKA

KAMPUS        : POLITEKNIK POS INDONESIA

LINK GITHUB

LINK REFERENSI

[http://linuxcentosproject.blogspot.co.id/2014/12/sejarah-centos.html](http://linuxcentosproject.blogspot.co.id/2014/12/sejarah-centos.html)

LINK PLAGIARISME