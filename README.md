# 1. Lihat daftar secara lengkap pada direktori aktif, belokkan tampilan standard output ke file baru.

![6 1](https://github.com/user-attachments/assets/52d1b1b6-edfa-435f-81c1-5bd4b2ee451e)

## -l: Menampilkan daftar file dalam format panjang, yang meliputi informasi seperti izin file, jumlah link, pemilik, grup, ukuran file, dan tanggal modifikasi.
## -a: Menampilkan semua file, termasuk file tersembunyi (file atau direktori yang namanya diawali dengan titik).
## > daftar_direktori.txt: Bagian ini berarti output dari perintah ls -la akan disimpan ke dalam file bernama daftar_direktori.txt, bukan ditampilkan di layar. Jadi, seluruh daftar direktori yang dihasilkan oleh perintah tersebut akan ditulis ke file tersebut.

# 2. Lihat daftar secara lengkap pada direktori /etc/paswd, belokkan tampilan standard output ke file baru tanpa menghapus file baru sebelumnya.

![6 2](https://github.com/user-attachments/assets/20271e9b-9d5e-43bb-9004-27f9e89ecf58)

## ls -la /etc/passwd: Perintah ini akan menampilkan informasi tentang file /etc/passwd dengan format panjang (-l), termasuk izin file, pemilik, grup, ukuran, dan waktu terakhir dimodifikasi.
## >> daftar_direktori.txt: Ini berarti hasil dari perintah di atas akan ditambahkan (append) ke dalam file daftar_direktori.txt, bukan menimpanya. Jika file tersebut sudah ada, hasil akan ditambahkan di akhir file.

# 3. Urutkan file baru dengan cara membelokkan standard input.

![6 3](https://github.com/user-attachments/assets/232e363b-9de5-4b98-b890-61fe4b1cc937)

## sort < daftar_direktori.txt: Ini berarti isi dari file daftar_direktori.txt dibaca dan diurutkan secara alfabetis. Perintah sort mengambil input dari file yang disebutkan dengan simbol < dan menampilkan hasil yang sudah diurutkan di terminal.

# 4. Urutkan file baru dengan cara membelokkan standard input dan standard output ke file baru.urut.

![6 4](https://github.com/user-attachments/assets/e2eba739-3a23-40b7-b9bf-99cbe77dba1d)

## sort: Ini adalah perintah utama, yang mengurutkan baris teks
## < daftar_direktori.txt: Ini mengalihkan isi file "daftar_direktori.txt" sebagai input ke perintah sort 
## > baru.urut: Ini mengalihkan output dari perintah sort ke file baru bernama "baru.urut"

# 5. Buatlah direktori latihan6 sebanyak 2 kali dan belokkan standard error ke file rmdirerror.txt.

![6 5](https://github.com/user-attachments/assets/bb6b24d5-0d53-4cd1-98ea-6f711bb8f5f6)

## mkdir latihan6: Perintah ini mencoba membuat sebuah direktori baru bernama "latihan6".
## 2> rmdirror.txt: Bagian ini mengarahkan output error (stderr, yang ditandai dengan '2') ke file bernama "rmdirror.txt". Jika ada pesan error saat membuat direktori, pesan tersebut akan disimpan dalam file ini alih-alih ditampilkan di layar.
## ayudiah@ayudiah-VirtualBox:~$ mkdir latihan6 Ini adalah perintah sederhana untuk membuat direktori bernama "latihan6".

# 6. Urutkan kalimat berikut : 
### Jakarta 
### Bandung 
### Surabaya 
### Padang 
### Palembang 
### Lampung 
### Dengan menggunakan notasi here document (<@@@ …@@@)

![6 6](https://github.com/user-attachments/assets/11f09040-51f2-400c-bb2f-6513a9c230f6)

## Perintah yang dijalankan: sort <<@@ Ini menggunakan "here-document" (diawali dengan <<) untuk memasukkan teks langsung ke perintah sort. @@ adalah penanda akhir dari input.
## Input yang diberikan: Jakarta, Bandung, Surabaya, Padang, Palembang, Lampung @@
## Daftar kota-kota dimasukkan, diakhiri dengan @@ untuk menandai akhir input.
## Output yang dihasilkan:, Bandung, Jakarta, Lampung, Padang, Palembang, Surabaya Ini adalah hasil pengurutan alfabetis dari daftar kota yang dimasukkan.
## Perintah sort secara default mengurutkan baris-baris teks secara alfabetis (ASCII). Dalam kasus ini, daftar kota-kota diurutkan dari A ke Z, menghasilkan daftar yang terurut seperti yang ditampilkan di bagian bawah gambar.

# 7. Hitung jumlah baris, kata dan karakter dari file baru.urut dengan menggunakan filter dan tambahkan data tersebut ke file baru.

![6 7](https://github.com/user-attachments/assets/07c3cc4e-31cd-4bb6-b88f-5c621bf6fd1c)

## wc: adalah perintah "word count" yang digunakan untuk menghitung jumlah baris, kata, dan karakter dalam sebuah file
## baru.urut: adalah nama file yang akan dihitung
## >>: operator ini digunakan untuk menambahkan (append) output ke file, bukan menimpa isinya
## daftar_direktori.txt: adalah file tujuan dimana hasil perhitungan akan ditambahkan

# 8. Gunakan perintah di bawah ini dan perhatikan hasilnya.
### $ cat /etc/passwd | sort | pr –n | grep tty03 
### $ find /etc –print | head 
### $ head /etc/passwd | tail –5 | sort

![6 82](https://github.com/user-attachments/assets/4cbad4b5-8612-49e0-a3da-ee1af5837c7d)

## cat /etc/passwd | sort | pr -n | grep tty03: Menampilkan isi file /etc/passwd, Mengurutkannya, Menambahkan nomor baris dengan pr -n, Mencari baris yang mengandung "tty03"
## find /etc -print | head: Perintah ini mencari semua file di direktori /etc dan menampilkan 10 hasil pertama.

![6 81](https://github.com/user-attachments/assets/416565e1-5574-4e2b-8c32-18b8472f302a)  

## Perintah ini menampilkan isi file /etc/passwd dan mengurutkannya secara alfabetis.

![6 8](https://github.com/user-attachments/assets/a586cd74-c909-459a-94bb-8ba3d6c76dbf)

## cat /etc/passwd : Perintah ini menampilkan isi file /etc/passwd tanpa modifikasi.
### File /etc/passwd berisi informasi akun pengguna pada sistem Linux, termasuk:
#### Nama pengguna
#### UID (User ID)
#### GID (Group ID)
#### Direktori home
#### Shell default

# 9. Gunakan perintah $ who | cat | cat | sort | pr | head | cat | tail dan perhatikan hasilnya.

![6 9](https://github.com/user-attachments/assets/389ddab1-d48b-4e5c-8303-b5607bad4bd3)

## 2024-09-12 15:08 : Ini adalah header yang ditambahkan oleh perintah pr, menunjukkan tanggal dan nomor halaman. ayudiah  tty7         
## 2024-09-05 15:00 (:0): Ini adalah informasi login pengguna:

#### Username: ayudiah
#### Terminal: tty7 (biasanya menunjukkan sesi grafis)
#### Waktu login: 2024-09-05 15:00
#### (:0) menunjukkan display grafis lokal
### Perintah who menampilkan informasi tentang pengguna yang sedang login.
### Perintah-perintah berikutnya memproses output ini, meskipun sebagian besar tidak mengubah isinya secara signifikan.
### sort mengurutkan output (meski dalam kasus ini hanya ada satu baris).
### pr menambahkan header dengan tanggal dan nomor halaman.
### head dan tail digunakan untuk mengambil bagian awal dan akhir output, yang dalam kasus ini menghasilkan seluruh output karena hanya ada sedikit baris.
