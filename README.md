# IT-Insight Mini Quiz

## Deskripsi

Aplikasi capstone berbasis Command Line Interface (CLI) menggunakan bahasa Python bernama "IT-Insight Mini Quiz". Proyek ini dikembangkan untuk mengatasi masalah utama pelajar IT, yaitu kesenjangan teori hafalan vs praktik logika (*The Theory-Practice Gap*) dan kurangnya media evaluasi mandiri rendah tekanan (*Low-Stakes Self-Assessment*). Sistem ini mengelompokkan bank soal ke dalam 2 kategori besar dengan mekanika tingkat kesulitan berbasis pengetatan jumlah nyawa (Level 1: 4 nyawa, Level 2: 3 nyawa, Level 3: 1 nyawa). Target penggunanya adalah siswa/mahasiswa rumpun Teknologi Informasi (Pelajar IT) tingkat pemula yang ingin mengasah wawasan IT serta keterampilan pemrograman mereka, sekaligus membutuhkan alat ukur kesiapan pemahaman logika program khususnya Python.

---

## Fitur Utama

### 1. Fitur Wajib

* 
**Bank Soal:** Basis data penyimpanan soal multi-level yang menampung teks pertanyaan, pilihan ganda, dan kunci jawaban secara terstruktur.


* 
**Quiz Random:** Sistem pengacakan otomatis untuk urutan kemunculan soal maupun opsi pilihan jawaban (A, B, C, D) agar setiap sesi kuis yang dimainkan tetap dinamis.


* 
**Scoring (Kalkulasi Nilai):** Perhitungan skor akhir level secara otomatis berbasis persentase total jawaban yang benar setelah sesi kuis selesai.


* **Papan Peringkat (Leaderboard):** Fitur untuk menyusun, mengurutkan, dan menampilkan peringkat utama para pemain berdasarkan perolehan skor tertinggi.
* **Review Jawaban:** Fasilitas pasca-kuis untuk melihat kembali evaluasi lembar jawaban pemain dan mencocokkannya secara langsung dengan kunci jawaban yang benar.

### 2. Fitur Tambahan

* 
**Sistem Nyawa (Lives):** Mekanika simulasi tekanan yang membatasi toleransi kesalahan pemain berdasarkan tingkat kesulitan level (Level 1: 4 nyawa, Level 2: 3 nyawa, Level 3: 1 nyawa).


* 
**Fitur Kategori dan Perlevelan:** Sistem manajemen soal yang membagi kuis ke dalam 2 kategori utama (Wawasan Umum IT dan Tebak Code & Output Python) serta memetakan materi secara simetris ke dalam 3 tingkatan kesulitan (Level 1, 2, dan 3).



---

## Cara Menjalankan

1. Buka Google Colab
2. Upload file utama Python ke dalam penyimpanan *session*
3. Jalankan kode program langsung pada *cell* Colab

---

## Struktur Data

* 
**Katalog Soal:** Menggunakan *Dictionary multi-level* (Nested Dictionary) dengan pencarian konstan $O(1)$ berdasarkan pencocokan *key-value* dari input menu pengguna.


* **Riwayat Skor:** Menggunakan *List of Dictionary* untuk menampung seluruh data hasil pengerjaan kuis (nama, kategori, level, dan skor akhir).
* **Kategori:** Menggunakan objek *Set* untuk membuang elemen duplikat secara otomatis dalam pengelolaan daftar pilihan kategori.

---

## Algoritma yang Digunakan

* **Bubble Sort:** Digunakan untuk mengurutkan data riwayat skor secara menurun (*descending*) guna menyusun papan peringkat secara rapi.
* **Total Skor (Rekursi):** Menggunakan fungsi rekursif fungsional untuk menghitung akumulasi total nilai keseluruhan pemain yang terdata di dalam sistem.
* **Option Shuffling:** Mengacak urutan pilihan opsi jawaban di dalam dictionary kuis secara dinamis tanpa mengubah kunci jawaban asli.
* 
**Manipulasi ASCII:** Pelacakan sandi enkripsi kriptografi pergeseran bit karakter (Sandi Caesar) memanfaatkan fungsi `ord()` dan `chr()`.



---

## Identitas

* **Nama**: [Nama Anda]
* **NIM**: [NIM Anda]
* 
**Mata Kuliah**: Praktikum Fondasi Pemrograman - Media Evaluasi Mandiri Pelajar IT 


* **Dosen**: Tri Aji Nugroho, S.T., M.T.
* **Semester**: Genap 2025/2026
