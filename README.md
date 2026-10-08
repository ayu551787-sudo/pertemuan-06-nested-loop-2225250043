# Pertemuan 06 Nested Loop Python

**Nama:** Ayu Syarifatu Zahra
**NIM:** 2225250043
**Kelas:** 3B

## Tujuan

Menggunakan nested loop, pola, akumulasi, dan pencacahan dalam bahasa pemrograman Python.

## Cara Menjalankan

Jalankan program melalui terminal dengan perintah berikut:

```bash
python3 tugas/tabel_perkalian_dan_statistik.py
```

## Algoritma Tugas 3

Program ini menggunakan nested loop untuk menghasilkan tabel pasangan perkalian dengan ukuran `n × n`.

Langkah-langkah algoritma:

1. Membaca input nilai `n`.
2. Memvalidasi input agar nilai `n` positif.
3. Menggunakan loop luar untuk mengatur baris.
4. Menggunakan loop dalam untuk menghasilkan pasangan perkalian.
5. Menghitung jumlah nilai pada setiap baris menggunakan `total_baris`.
6. Menghitung jumlah seluruh nilai menggunakan `total_semua`.
7. Menghitung banyaknya hasil genap menggunakan `count_genap`.
8. Menampilkan hasil tabel dan statistik.

## Hasil Pengujian

Catat hasil pengujian program pada tabel berikut.

| No. | Input    | Hasil yang Diharapkan             | Keluaran Aktual | Status |
| --- | -------- | --------------------------------- | --------------- | ------ |
| 1   | `n = 3`  | Menghasilkan 9 pasangan perkalian | 36              | pas    |
| 2   | `n = 2`  | Menghasilkan 4 pasangan perkalian | 9               | pas    |
| 3   | `n = 0`  | Menampilkan pesan validasi input  | tidak terbaca   | pas    |
| 4   | `n = 1`  | Menampilkan pesan validasi input  | 1               | pas    |

## Analisis Efisiensi

Untuk input `n`, loop luar dijalankan sebanyak `n` kali dan loop dalam dijalankan sebanyak `n` kali untuk setiap iterasi loop luar.

Jumlah seluruh eksekusi pernyataan di dalam loop bersarang adalah:

`n × n = n²`

Dengan demikian, kompleksitas waktu program adalah **O(n²)**.

## Refleksi

Salah satu kesalahan yang dapat terjadi pada nested loop adalah tidak mereset variabel `total_baris` ketika memulai baris baru. Akibatnya, jumlah pada setiap baris dapat menjadi tidak tepat.

Cara memperbaikinya adalah dengan menginisialisasi `total_baris = 0` di awal setiap iterasi loop luar.
