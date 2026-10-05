# Pertemuan 06 - Nested Loop, Pola, Akumulasi, dan Pencacahan

## Identitas

- Nama: Fikri Yustiawan
- NIM: 2225250075
- Kelas: 3-E

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

```bash
python3 tugas/tabel_perkalian_dan_statistik.py
