# Lihat daftar secara lengkap pada direktori aktif, belokkan tampilan standard output ke file baru.

![6 1](https://github.com/user-attachments/assets/52d1b1b6-edfa-435f-81c1-5bd4b2ee451e)

## -l: Menampilkan daftar file dalam format panjang, yang meliputi informasi seperti izin file, jumlah link, pemilik, grup, ukuran file, dan tanggal modifikasi.
## -a: Menampilkan semua file, termasuk file tersembunyi (file atau direktori yang namanya diawali dengan titik).
## > daftar_direktori.txt: Bagian ini berarti output dari perintah ls -la akan disimpan ke dalam file bernama daftar_direktori.txt, bukan ditampilkan di layar. Jadi, seluruh daftar direktori yang dihasilkan oleh perintah tersebut akan ditulis ke file tersebut.

# Lihat daftar secara lengkap pada direktori /etc/paswd, belokkan tampilan standard output ke file baru tanpa menghapus file baru sebelumnya.

![6 2](https://github.com/user-attachments/assets/20271e9b-9d5e-43bb-9004-27f9e89ecf58)

## ls -la /etc/passwd: Perintah ini akan menampilkan informasi tentang file /etc/passwd dengan format panjang (-l), termasuk izin file, pemilik, grup, ukuran, dan waktu terakhir dimodifikasi.
## >> daftar_direktori.txt: Ini berarti hasil dari perintah di atas akan ditambahkan (append) ke dalam file daftar_direktori.txt, bukan menimpanya. Jika file tersebut sudah ada, hasil akan ditambahkan di akhir file.

# Urutkan file baru dengan cara membelokkan standard input.

![6 3](https://github.com/user-attachments/assets/232e363b-9de5-4b98-b890-61fe4b1cc937)

## sort < daftar_direktori.txt: Ini berarti isi dari file daftar_direktori.txt dibaca dan diurutkan secara alfabetis. Perintah sort mengambil input dari file yang disebutkan dengan simbol < dan menampilkan hasil yang sudah diurutkan di terminal.

# . Urutkan file baru dengan cara membelokkan standard input dan standard output ke file baru.urut.

![6 4](https://github.com/user-attachments/assets/e2eba739-3a23-40b7-b9bf-99cbe77dba1d)

## sort: Ini adalah perintah utama, yang mengurutkan baris teks
## < daftar_direktori.txt: Ini mengalihkan isi file "daftar_direktori.txt" sebagai input ke perintah sort > baru.urut: Ini mengalihkan output dari perintah sort ke file baru bernama "baru.urut"
