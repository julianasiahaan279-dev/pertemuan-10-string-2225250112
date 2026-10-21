# Pertemuan 10 - String dan Pengolahan Teks

Nama: Angelita Juliana Siahaan
NIM: 2225250112
Kelas: 3B

## Tujuan
Mengolah dan menormalisasi data teks dengan string Python.

## Cara Menjalankan
python tugas/normalisasi_data_mahasiswa.py

## Algoritma
1. Program membaca nama dan kode kelas sebagai string.
2. Nama dibersihkan dari spasi berlebih dengan strip dan split, digabung lagi dengan join, lalu diubah ke title case.
3. Nama yang sudah bersih dipecah menjadi list kata untuk menghitung jumlah kata dan mengambil huruf pertama tiap kata sebagai inisial.
4. Kode kelas diubah ke huruf besar, dipecah per kata, lalu digabung dengan tanda hubung.
5. Semua hasil ditampilkan dengan rapi.

## Test Case
| Input Nama | Input Kode | Hasil diharapkan | Hasil aktual | Status |
|------------|------------|------------------|--------------|--------|
| aan hendrayana | pmat a 2026 | Aan Hendrayana, PMAT-A-2026, 2, AH | Aan Hendrayana, PMAT-A-2026, 2, AH | Lulus |
| fATHIYYAH mUTHMAINNAH | kelas b | Fathiyyah Muthmainnah, KELAS-B, 2, FM | Fathiyyah Muthmainnah, KELAS-B, 2, FM | Lulus |
| BUDI | pmtk 01 | Budi, PMTK-01, 1, B | Budi, PMTK-01, 1, B | Lulus |
|   siti nur aisyah | kelas c | Siti Nur Aisyah, KELAS-C, 3, SNA | Siti Nur Aisyah, KELAS-C, 3, SNA | Lulus |

## Refleksi
## Refleksi
Masalah teks yang saya temukan adalah data nama dan kode kelas yang formatnya tidak konsisten, misalnya nama "  siti nur aisyah" yang memiliki spasi berlebih di depan dan huruf kecil semua, nama "fATHIYYAH mUTHMAINNAH" yang huruf besar dan kecilnya acak, serta kode kelas "pmat a 2026" yang masih huruf kecil dan dipisah spasi. Masalah ini saya perbaiki dengan strip() untuk menghapus spasi di awal dan akhir, split() lalu join() untuk merapikan spasi berlebih, title() untuk menyeragamkan kapitalisasi nama, serta upper() dan join dengan tanda hubung untuk kode kelas. Dari tugas ini saya juga memahami bahwa string bisa ditelusuri dengan indeks dan slicing seperti list, dan hasil split() berupa list kata yang bisa dihitung dengan len() serta diambil huruf pertamanya untuk inisial.