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
| 1 | **[Nama Anda]** | `[NIM Anda]` | `[@username-ketua]` | **Ketua Kelompok:** Manajemen repository, penurunan model matematis keseimbangan titik buhul, integrasi kode utama (`main`), dan finalisasi dokumentasi. |
| 2 | **[Nama Anggota 2]** | `[NIM Anggota 2]` | `[@username-2]` | **Anggota:** Penentuan geometri rangka (misal: Pratt/Howe/Warren), skema pembebanan, penyusunan data parameter (`data/`), dan validasi analitik/pustaka (`scipy`/`numpy`). |
| 3 | **[Nama Anggota 3]** | `[NIM Anggota 3]` | `[@username-3]` | **Anggota:** Implementasi metode **Sistem Persamaan Linier (SPL)** (Eliminasi Gauss / Dekomposisi LU) untuk menghitung gaya tiap batang (`src/spl_gauss.py`). |
| 4 | **[Nama Anggota 4]** | `[NIM Anggota 4]` | `[@username-4]` | **Anggota:** Implementasi metode **SPL Iteratif (Gauss-Seidel)** sebagai pembanding kestabilan/kecepatan serta **Akar Persamaan** untuk mencari beban kritis (`src/akar_beban_kritis.py`). |
| 5 | **[Nama Anggota 5]** | `[NIM Anggota 5]` | `[@username-5]` | **Anggota:** Implementasi metode **Regresi** (hubungan beban vs gaya batang), analisis galat, dan pembuatan visualisasi grafik/tabel (`src/regresi_plot.py` & `figures/`). |

---

## 3. Project Progress
Catatan perkembangan proyek mingguan (Pertemuan 8 – Pertemuan 12):

| Week | Activities | Status | Person in Charge |
| :--- | :--- | :--- | :--- |
| **P8** | Pembuatan repository GitHub, pembagian tugas, penentuan tipe rangka atap (Truss) & asumsi parameter | Completed | All Members |
| **P9** | Penurunan model matematis keseimbangan gaya ($\sum F_x = 0, \sum F_y = 0$) & penyusunan matriks kekakuan/keseimbangan | In Progress | [Nama Anda] & [Nama Anggota 2] |
| **P10** | Implementasi kode Python untuk metode SPL (Gauss/LU & Gauss-Seidel) dan Akar Persamaan | Not Started | [Nama Anggota 3] & [Nama Anggota 4] |
| **P11** | Implementasi Regresi, validasi hasil dengan `numpy.linalg.solve`, dan analisis galat | Not Started | [Nama Anggota 5
