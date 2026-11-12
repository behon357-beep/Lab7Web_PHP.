# LAPORAN PRAKTIKUM 7
## PEMROGRAMAN SERVER-SIDE DENGAN PHP

### 1. Identitas Praktikum

- **Mata Kuliah:** Pemrograman Web
- **Topik:** Pemrograman Server-Side dengan PHP
- **Nama:** Maulana Akbar
- **NIM:** 312510381
- **Program Studi:** Teknik Informatika

---

### 2. Tujuan Praktikum

Praktikum ini bertujuan untuk memahami dasar pemrograman PHP sebagai bahasa pemrograman server-side. Selain itu, praktikum ini dilakukan untuk mempelajari penggunaan variabel, operator, percabangan, perulangan, array, function, serta pemrosesan data menggunakan form HTML dengan metode GET dan POST.

### 3. Persiapan Lingkungan Praktikum

Perangkat dan aplikasi yang digunakan:

1. Visual Studio Code sebagai editor untuk menulis kode program.
2. XAMPP sebagai server lokal.
3. Apache sebagai web server untuk menjalankan file PHP.
4. Browser untuk melihat hasil program.

**Cara menjalankan program:**

1. Membuat folder proyek bernama `Lab7Web_php` di dalam folder `htdocs`.
2. Membuat file PHP sesuai dengan latihan yang dikerjakan.
3. Membuka aplikasi XAMPP dan mengaktifkan Apache.
4. Membuka browser dan mengakses alamat `http://localhost/Lab7Web_php/`.
5. Memilih file latihan yang ingin dijalankan.

---

# 4. Hasil Praktikum (Poin E)

## Latihan 1 – Menjalankan PHP

**Tujuan:**

Latihan pertama bertujuan untuk memahami cara menjalankan kode PHP melalui web server lokal menggunakan XAMPP.

**Penjelasan kode:**

Pada latihan ini digunakan struktur dasar HTML yang digabungkan dengan kode PHP. Perintah `echo` digunakan untuk menampilkan teks ke halaman browser. Selain itu, fungsi `date()` digunakan untuk menampilkan waktu server berdasarkan format tanggal dan waktu yang ditentukan.

**Hasil pengujian:**

Program berhasil menampilkan tulisan "Belajar PHP", pesan bahwa PHP berhasil dijalankan, serta waktu server saat halaman dibuka.

**Screenshot hasil:**
<img width="268" height="150" alt="Screenshot 2026-11-12 093203" src="https://github.com/user-attachments/assets/33f003f1-27ee-49d5-bd20-30c79488b499" />


---

## Latihan 2 – Variabel, Operator, dan Percabangan

**Tujuan:**

Memahami penggunaan variabel, operator aritmatika, dan percabangan untuk melakukan perhitungan nilai akhir mahasiswa.

**Penjelasan kode:**

Program menggunakan beberapa variabel, yaitu `$nama`, `$tugas`, `$uts`, dan `$uas` untuk menyimpan data mahasiswa dan nilai yang diperoleh.

Perhitungan nilai akhir dilakukan menggunakan operator perkalian dan penjumlahan dengan bobot tugas 30%, UTS 30%, dan UAS 40%.

Selanjutnya, struktur percabangan `if`, `elseif`, dan `else` digunakan untuk menentukan predikat berdasarkan nilai akhir yang diperoleh.

Fungsi `number_format()` digunakan untuk mengatur tampilan angka menjadi dua angka di belakang koma.

**Hasil pengujian:**

Program berhasil menghitung nilai akhir mahasiswa dan menampilkan predikat berdasarkan ketentuan nilai yang telah dibuat.

**Screenshot hasil:**

<img width="242" height="72" alt="Screenshot 2026-11-12 094051" src="https://github.com/user-attachments/assets/9b9e83c1-1bcd-4b1d-ae2a-a1727c8dfe72" />


---

## Latihan 3 – Perulangan dan Array

**Tujuan:**

Memahami penggunaan array untuk menyimpan beberapa data dan perulangan `foreach` untuk menampilkan seluruh data tersebut.

**Penjelasan kode:**

Pada latihan ini digunakan variabel `$mahasiswa` yang berisi beberapa nama mahasiswa dalam bentuk array.

Perulangan `foreach` digunakan untuk mengambil setiap data nama dari array dan menyimpannya sementara ke dalam variabel `$nama`.

Perintah `echo` digunakan untuk menampilkan setiap nama ke halaman browser. Sementara itu, tag HTML `<ol>` dan `<li>` digunakan untuk membuat daftar nama secara berurutan.

Fungsi `htmlspecialchars()` digunakan untuk mengamankan teks sebelum ditampilkan ke halaman HTML.

**Hasil pengujian:**

Program berhasil menampilkan seluruh nama mahasiswa yang tersimpan dalam array menggunakan daftar bernomor. Pengujian dilakukan dengan menambahkan minimal tiga nama mahasiswa.

**Screenshot hasil:**

<img width="517" height="205" alt="Screenshot 2026-11-12 095651" src="https://github.com/user-attachments/assets/f0655c38-d734-4528-b375-ad4b40b876f1" />


---

## Latihan 4 – Membuat Function

**Tujuan:**

Memahami cara membuat dan menggunakan function dalam PHP untuk melakukan proses perhitungan secara terstruktur.

**Penjelasan kode:**

Pada latihan ini dibuat function bernama `hitungDiskon()` yang memiliki dua parameter, yaitu `$harga` dan `$persen`.

Variabel `$potongan` digunakan untuk menghitung jumlah diskon berdasarkan harga dan persentase diskon yang diberikan.

Perintah `return` digunakan untuk mengembalikan hasil pengurangan harga awal dengan potongan diskon.

Function kemudian dipanggil menggunakan nilai harga Rp150.000 dan diskon 10%. Fungsi `number_format()` digunakan untuk menampilkan hasil harga dalam format Rupiah.

**Hasil pengujian:**

Program berhasil menghitung harga setelah diskon. Dari harga awal Rp150.000 dengan diskon 10%, diperoleh harga akhir sebesar Rp135.000.

**Screenshot hasil:**

<img width="350" height="47" alt="Screenshot 2026-11-12 100300" src="https://github.com/user-attachments/assets/338cb3a6-b551-4f30-8a35-36293b3f200e" />


---

## Latihan 5 – Memproses Form dengan GET

**Tujuan:**

Memahami cara menerima dan memproses data yang dikirimkan melalui form HTML menggunakan metode GET.

**Penjelasan kode:**

Pada latihan ini dibuat form pencarian yang memiliki input dengan nama `kata` dan tombol Cari.

Atribut `method="GET"` digunakan agar data dikirim melalui parameter URL. Sementara itu, atribut `action=""` menunjukkan bahwa data akan diproses pada halaman yang sama.

PHP menggunakan `isset($_GET["kata"])` untuk memeriksa apakah data pencarian telah dikirim.

Fungsi `trim()` digunakan untuk menghapus spasi di awal dan akhir input. Selanjutnya, `htmlspecialchars()` digunakan untuk mengamankan teks sebelum ditampilkan.

**Hasil pengujian:**

Program berhasil menerima kata kunci dari pengguna dan menampilkan kembali kata tersebut pada halaman browser. Setelah tombol Cari ditekan, parameter pencarian juga terlihat pada URL browser.

**Screenshot hasil:**

<img width="877" height="181" alt="image" src="https://github.com/user-attachments/assets/5c013475-f75c-419c-924e-a0ff387bc664" />


---

## Latihan 6 – Memproses Form dengan POST

**Tujuan:**

Memahami cara mengirim dan memproses data dari form HTML menggunakan metode POST.

**Penjelasan kode:**

Pada latihan ini dibuat form yang terdiri dari dua input, yaitu nama dan program studi. Kedua input tersebut memiliki atribut `required` agar pengguna diwajibkan mengisi data.

Atribut `method="POST"` digunakan untuk mengirimkan data melalui body permintaan HTTP.

PHP menggunakan `$_SERVER["REQUEST_METHOD"]` untuk memeriksa apakah halaman menerima permintaan POST.

Data yang dikirim kemudian diambil menggunakan `$_POST`, sedangkan fungsi `trim()` digunakan untuk menghapus spasi yang tidak diperlukan.

Percabangan `if` digunakan untuk memeriksa apakah nama atau program studi masih kosong. Jika terdapat data kosong, program menampilkan pesan kesalahan. Jika semua data sudah diisi, program menampilkan ringkasan data menggunakan `htmlspecialchars()`.

**Hasil pengujian:**

Program berhasil menerima dan menampilkan data nama serta program studi ketika seluruh kolom diisi. Program juga menampilkan pesan kesalahan apabila terdapat data yang tidak sesuai.

**Screenshot hasil:**

<img width="733" height="272" alt="Screenshot 2026-11-12 103503" src="https://github.com/user-attachments/assets/3103115f-caa6-4bc6-9091-608b22482831" />


---

## Latihan 7 – Pengolahan Data Sederhana

**Tujuan:**

Memahami cara mengolah data dari form HTML menggunakan PHP untuk melakukan perhitungan subtotal transaksi barang.

**Penjelasan kode:**

Pada latihan ini dibuat form yang terdiri dari tiga input, yaitu nama barang, harga, dan jumlah.

Data dikirim menggunakan metode POST dan diterima melalui variabel `$_POST`.

Fungsi `trim()` digunakan untuk membersihkan input nama barang. Selanjutnya, program melakukan validasi menggunakan `is_numeric()` untuk memeriksa harga dan `ctype_digit()` untuk memeriksa jumlah.

Percabangan digunakan untuk memastikan nama barang tidak kosong, harga berupa angka dan tidak negatif, serta jumlah berupa bilangan bulat minimal satu.

Jika seluruh data memenuhi ketentuan, harga dan jumlah dikonversi menggunakan tipe data `float` dan `int`.

Selanjutnya, subtotal dihitung menggunakan rumus:

Subtotal = Harga × Jumlah

Fungsi `number_format()` digunakan untuk menampilkan hasil perhitungan dalam format Rupiah, sedangkan `htmlspecialchars()` digunakan untuk mengamankan nama barang sebelum ditampilkan.

**Hasil pengujian:**

Program berhasil menerima data transaksi barang, melakukan validasi input, menghitung subtotal, dan menampilkan ringkasan transaksi.

Pengujian dilakukan dengan memasukkan harga desimal, jumlah nol, jumlah negatif, serta data yang tidak sesuai untuk memastikan validasi berjalan dengan baik.

**Screenshot hasil:**

<img width="921" height="150" alt="Screenshot 2026-11-12 104555" src="https://github.com/user-attachments/assets/c6da0e85-52db-47c5-bf8a-3ff7d2013b46" />


---
## Mini Project – Aplikasi Formulir Data Mahasiswa

**Tujuan:**

Membuat aplikasi formulir data mahasiswa menggunakan PHP dengan metode POST untuk menerima, memvalidasi, dan menampilkan data mahasiswa.

**Penjelasan Kode:**

Program memiliki lima input, yaitu nama, NIM, program studi, semester, dan email. Data dikirim menggunakan metode POST kemudian diperiksa melalui validasi server-side. Fungsi `filter_var()` digunakan untuk memvalidasi format email, sedangkan `ctype_digit()` digunakan untuk memeriksa input semester. Jika seluruh data valid, program akan menampilkan ringkasan data mahasiswa. Jika terdapat kesalahan, program akan menampilkan pesan validasi.

**Hasil Pengujian:**

Program berhasil menerima dan menampilkan data mahasiswa apabila seluruh input sesuai dengan ketentuan. Jika terdapat input kosong, format email salah, atau semester di luar rentang 1–14, program akan menampilkan pesan kesalahan.

**Screenshot Hasil:**


<img width="437" height="532" alt="image" src="https://github.com/user-attachments/assets/000cd2f1-0b6a-4490-a112-d056dfefc82c" />

<img width="738" height="377" alt="Screenshot 2026-11-12 105145" src="https://github.com/user-attachments/assets/053c2282-32c5-4e5c-8787-abb02d964d0a" />


# 5. Kesimpulan

Berdasarkan praktikum yang telah dilakukan, dapat disimpulkan bahwa PHP dapat digunakan untuk memproses data pada sisi server dan menampilkan hasilnya melalui browser.

Melalui tujuh latihan yang telah dikerjakan, saya mempelajari penggunaan variabel, operator, percabangan, perulangan, array, function, serta pemrosesan form menggunakan metode GET dan POST.

Selain itu, praktikum ini memberikan pemahaman mengenai pentingnya validasi dan sanitasi input untuk memastikan data yang diterima sesuai dengan ketentuan serta aman ketika ditampilkan kembali ke halaman browser.

Dengan menyelesaikan praktikum ini, saya memperoleh pemahaman dasar mengenai bagaimana PHP bekerja dalam mengolah data pengguna menjadi sebuah aplikasi web sederhana.
