# luckyDOS

## Deskripsi Proyek

Lucky DOS adalah skrip berbasis Python untuk menguji serangan Distributed Denial of Service (DDoS). Alat ini memiliki tiga jenis serangan: SYNFLOOD, REQUEST, dan Pyslow (mirip dengan Slowloris).

## Penggunaan

Skrip dapat dijalankan dengan berbagai opsi untuk menentukan IP/domain target, port, jumlah thread, dan jenis serangan.
Gunakan skrip ini dengan hati-hati dan hanya untuk tujuan pembelajaran. Saya tidak bertanggung jawab atas segala kerusakan atau pelanggaran hukum yang mungkin terjadi akibat penggunaan skrip ini.

## Module Yang Dibutuhkan

-   termcolor
-   colorama

### Perintah

-   `-t`, `--target` - Target web, misalnya "contoh.com"
-   `-v`, `--version` - Menampilkan versi program
-   `-h`, `--help` - Memunculkan bantuan

-   `-d <ip|domain>` - Menentukan target seperti alamat IP atau nama domain
-   `-t <float>` Mengatur timeout untuk socket
-   `-T <int>` Mengatur jumlah thread untuk koneksi (default = 1000)
-   `-p <int>` Menentukan port target (default = 80) |Hanya diperlukan untuk serangan pyslow|
-   `-s <int>` Mengatur waktu tidur untuk rekoneksi
-   `-i <ip address>` Menentukan IP spoofed kecuali menggunakan IP palsu
-   `-Request ` Mengaktifkan target permintaan
-   `-Synflood ` Mengaktifkan serangan synflood
-   `-Pyslow` Mengaktifkan serangan pyslow
-   `--fakeip` Opsi untuk membuat IP palsu jika tidak menentukan IP spoofed

### Contoh Penggunaan

Jalankan perintah berikut untuk menjalankan skrip:

```sh
./luckyDOS -t [target] -p [port] -t [jumlah threads]
```

## Struktur Proyek

-   `luckyDOS.py`
-   `README.md`

### Penjelasan File

#### `luckyDOS.py`

Skrip utama yang mengimplementasikan tiga jenis serangan DDoS (SYNFLOOD, REQUEST, dan Pyslow). Menggunakan modul termcolor dan colorama untuk memberikan output berwarna di terminal.

#### `README.md`

Berisi dokumentasi proyek, termasuk deskripsi, cara penggunaan, dan informasi penting lainnya.

## Peringatan

Skrip ini dibuat hanya untuk tujuan pembelajaran dan penelitian. Penggunaan skrip ini pada situs web tanpa izin adalah ilegal dan dapat menyebabkan masalah hukum. Saya tidak bertanggung jawab atas segala kerusakan, pelanggaran hukum, atau konsekuensi lain yang mungkin terjadi akibat penggunaan skrip ini.

**Date**: Jul 6, 2019
