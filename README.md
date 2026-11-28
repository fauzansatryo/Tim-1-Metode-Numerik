# Analisis Gaya pada Struktur Rangka Batang (Truss) Atap

## 1. Project Information
* **Project Title:** Analisis Gaya pada Struktur Rangka Batang (Truss) Atap
* **Course:** Metode Numerik (Semester Ganjil 2026/2027)
* **Group Number:** Tim 1
* **Project Description:** Proyek ini bertujuan untuk memodelkan dan menganalisis distribusi gaya tarik dan tekan pada struktur rangka batang (truss) atap baja bentang lebar akibat beban mati, beban hidup, dan beban angin. Penyelesaian dilakukan menggunakan minimal tiga metode numerik (Sistem Persamaan Linier, Akar Persamaan, dan Regresi) untuk mengidentifikasi batang kritis dan batas beban maksimal yang aman.

---

## 2. Team Members
Berikut adalah pembagian peran dan tanggung jawab untuk masing-masing anggota tim (5 orang):

| No | Name | NIM | GitHub Username | Role & Responsibility |
| :--- | :--- | :--- | :--- | :--- |
| 1 | **Muhammad Fauzan Satryo** | 20250204018` | `fauzansatryo` | **Ketua Kelompok:** Manajemen repository, penurunan model matematis keseimbangan titik buhul, integrasi kode utama (`main`), dan finalisasi dokumentasi. |
| 2 | **Raka Ardian Nugraha** | `2025020420` | `rakaadriannugraha99` | **Anggota:** Penentuan geometri rangka (misal: Pratt/Howe/Warren), skema pembebanan, penyusunan data parameter (`data/`), dan validasi analitik/pustaka (`scipy`/`numpy`). |
| 3 | **Retnadila Endah Priyono** | `20250204021` | `RetnadilaEndahPriyono` | **Anggota:** Implementasi metode **Sistem Persamaan Linier (SPL)** (Eliminasi Gauss / Dekomposisi LU) untuk menghitung gaya tiap batang (`src/spl_gauss.py`). |
| 4 | **Novita Indri Ramadhani** | `20250204002` | `` | **Anggota:** Implementasi metode **SPL Iteratif (Gauss-Seidel)** sebagai pembanding kestabilan/kecepatan serta **Akar Persamaan** untuk mencari beban kritis (`src/akar_beban_kritis.py`). |
| 5 | **Trista Olivia** | `20250204012` | `TristaOlivia` | **Anggota:** Implementasi metode **Regresi** (hubungan beban vs gaya batang), analisis galat, dan pembuatan visualisasi grafik/tabel (`src/regresi_plot.py` & `figures/`). |

---

## 3. Project Progress
Catatan perkembangan proyek mingguan (Pertemuan 8 – Pertemuan 12):

| Week | Activities | Status | Person in Charge |
| :--- | :--- | :--- | :--- |
| **P8** | Pembuatan repository GitHub, pembagian tugas, penentuan tipe rangka atap (Truss) & asumsi parameter | Completed | All Members |
| **P9** | Penurunan model matematis keseimbangan gaya ($\sum F_x = 0, \sum F_y = 0$) & penyusunan matriks kekakuan/keseimbangan | In Progress | [Nama Anda] & [Nama Anggota 2] |
| **P10** | Implementasi kode Python untuk metode SPL (Gauss/LU & Gauss-Seidel) dan Akar Persamaan | Not Started | [Nama Anggota 3] & [Nama Anggota 4] |
| **P11** | Implementasi Regresi, validasi hasil dengan `numpy.linalg.solve`, dan analisis galat | Not Started | [Nama Anggota 5
