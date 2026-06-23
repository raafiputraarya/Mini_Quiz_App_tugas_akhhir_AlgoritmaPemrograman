# Mini_Quiz_App_tugas_akhhir_AlgoritmaPemrograman

# Sistem Perpustakaan Mini UAI

---

## Deskripsi Proyek

**Sistem Perpustakaan Mini UAI** adalah sebuah aplikasi berbasis antarmuka konsol (CLI) yang dikembangkan menggunakan bahasa pemrograman Python. Sistem ini dirancang secara khusus untuk memfasilitasi dan mengelola operasional perpustakaan skala kecil secara digital. Aplikasi ini merupakan luaran dari proyek akhir untuk mata kuliah Algoritma dan Pemrograman di Universitas Al Azhar Indonesia, yang bertujuan untuk mendemonstrasikan pemahaman praktis mengenai struktur data, algoritma dasar, dan manajemen file.

---

## Fitur Utama

Aplikasi ini mencakup serangkaian fungsionalitas inti untuk manajemen perpustakaan modern:

* **Manajemen Katalog:** Kemampuan untuk menambah buku baru ke dalam pangkalan data atau menghapus buku yang sudah tidak relevan.
* **Mesin Pencari:** Fitur pencarian presisi yang memungkinkan pengguna menemukan buku berdasarkan *Judul*, *Pengarang*, atau *Kategori*.
* **Sirkulasi Buku:** Sistem otomatisasi untuk mencatat transaksi peminjaman dan pengembalian buku, lengkap dengan pembaruan status ketersediaan.
* **Dasbor Statistik:** Representasi metrik komprehensif mengenai kondisi perpustakaan, seperti total buku, buku yang dipinjam, dan buku yang tersedia.
* **Penyimpanan Persisten:** Data katalog tidak akan hilang ketika program ditutup karena seluruh rekaman transaksi dan katalog disimpan secara otomatis ke dalam file lokal.

---

## Panduan Menjalankan Program

Aplikasi ini dirancang agar mudah dieksekusi di lingkungan *cloud* maupun lokal. Berikut adalah panduan menjalankan program menggunakan **Google Colab**:

1. Buka *platform* Google Colab melalui *browser* Anda.
2. Unggah file `main.py` ke dalam sistem *file* penyimpanan *session* Colab Anda.
3. Buat sebuah sel (*cell*) baru dan jalankan perintah: `!python main.py`
4. Sebagai alternatif, Anda dapat menyalin (*copy*) seluruh kode sumber dan menempelkannya (*paste*) langsung ke dalam sel eksekusi Colab untuk dijalankan secara langsung.

---

## Arsitektur Sistem

Pengembangan aplikasi ini didasarkan pada implementasi spesifik dari struktur data dan algoritma berikut untuk memastikan efisiensi ruang dan waktu:

### Struktur Data

* **Katalog Utama:** Menggunakan struktur *Dictionary* dengan kompleksitas waktu akses yang cepat, di mana `key` adalah `id_buku` dan `value` berupa objek `data_buku`.
* **Entitas Buku:** Setiap buku direpresentasikan sebagai *Dictionary* terpisah yang menyimpan atribut detail berupa `judul`, `pengarang`, `tahun`, dan `status`.

### Algoritma

* **Pencarian Data:** Mengimplementasikan algoritma *Linear Search* untuk melakukan iterasi pencarian dan pencocokan parameter string (judul, pengarang, kategori) secara berurutan di dalam katalog.
* **Pengurutan Data:** Memanfaatkan fungsi *Built-in Sort* dari Python yang sangat teroptimasi untuk menyusun dan menampilkan daftar katalog perpustakaan secara alfabetis atau kronologis.

---

## Identitas Pengembang

| Informasi | Keterangan |
| --- | --- |
| **Nama** | [Nama Anda] |
| **NIM** | [NIM Anda] |
| **Mata Kuliah** | Algoritma dan Pemrograman (3 SKS) |
| **Dosen Pengampu** | Tri Aji Nugroho, S.T., M.T. |
| **Semester** | Genap 2025/2026 |
| **Institusi** | Universitas Al Azhar Indonesia |

