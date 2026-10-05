# Pertemuan-06-nested-loop-2225250075

| **Keterangan** | **Data** |
|---|---|
| **Nama** | Fikri Yustiawan |
| **NIM** | 2225250075 |
| **Kelas** | 3-E |
| **Jurusan** | Pendidikan Matematika |

## Tujuan

Pada pertemuan ini mempelajari penggunaan nested loop, pola, akumulasi, dan pencacahan dalam Python.

Tugas yang dibuat adalah program Tabel Perkalian dan Statistik menggunakan nested loop.

## Struktur Program

Program berada pada file:

`tugas/tabel_perkalian_dan_statistik.py`

Program membuat tabel perkalian berukuran n × n dan menghitung:
- Total seluruh hasil perkalian.
- Banyak hasil perkalian yang genap.
- Jumlah hasil perkalian pada setiap baris.

## Algoritma

1. Membaca nilai `n` dari input.
2. Memastikan nilai `n` merupakan bilangan positif.
3. Jika `n <= 0`, program meminta input kembali sampai mendapatkan nilai positif.
4. Membuat variabel `total_semua = 0` untuk menyimpan total seluruh hasil.
5. Membuat variabel `count_genap = 0` untuk menghitung banyak hasil genap.
6. Menggunakan nested loop:
   - Perulangan luar untuk baris `i`.
   - Perulangan dalam untuk kolom `j`.
7. Menghitung hasil perkalian `i * j`.
8. Menambahkan hasil perkalian ke jumlah baris.
9. Menambahkan hasil perkalian ke total seluruh hasil.
10. Mengecek apakah hasil perkalian merupakan bilangan genap.
11. Menampilkan jumlah setiap baris.
12. Setelah semua perulangan selesai, menampilkan total seluruh hasil dan banyak hasil genap.

## Cara Menjalankan

Jalankan program dengan perintah:

``bash
python3 tugas/tabel_perkalian_dan_statistik.py``

## Hasil Pengujian

| Input | Hasil yang Diharapkan | Keluaran Aktual | Status |
|---|---|---|---|
| `n = 1` | Total seluruh hasil = 1, hasil genap = 0 | Total seluruh hasil = 1, hasil genap = 0 | Berhasil |
| `n = 2` | Total seluruh hasil = 9, hasil genap = 3 | Total seluruh hasil = 9, hasil genap = 3 | Berhasil |
| `n = 3` | Total seluruh hasil = 36, hasil genap = 5 | Total seluruh hasil = 36, hasil genap = 5 | Berhasil |

## Analisis Efisiensi

Untuk input `n`, loop dalam berjalan sebanyak `n` kali untuk setiap iterasi loop luar.

Karena loop luar juga berjalan sebanyak `n` kali, maka badan loop dalam berjalan sebanyak:

`n × n = n²`

Jadi, kompleksitas waktu program adalah `O(n²)`.

## Refleksi

Salah satu kesalahan yang dapat terjadi pada nested loop adalah menempatkan variabel `total_baris` di luar loop luar. Jika dilakukan, jumlah setiap baris akan terus terakumulasi dan tidak dimulai kembali dari nol.

Cara memperbaikinya adalah menempatkan `total_baris = 0` di dalam loop luar sebelum loop dalam dimulai, sehingga setiap baris memiliki akumulator sendiri.

## Exit Ticket

- Hal yang paling menentukan jumlah iterasi nested loop adalah nilai `n` dan jumlah perulangan pada loop luar dan loop dalam.

- Perbedaan akumulasi per baris dan akumulasi keseluruhan adalah akumulasi per baris digunakan untuk menghitung jumlah hasil pada satu baris dan direset setiap pergantian baris, sedangkan akumulasi keseluruhan terus menjumlahkan semua hasil dari seluruh baris.

- Bagian program Pertemuan 6 yang paling tepat dijadikan fungsi pada Pertemuan 7 adalah bagian pembuatan tabel perkalian dan perhitungan statistik, karena bagian tersebut memiliki proses yang jelas dan dapat dipisahkan menjadi fungsi agar program lebih terstruktur dan mudah digunakan kembali.
