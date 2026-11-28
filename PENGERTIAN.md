
## 10. Rencana Validasi

Validasi dilakukan untuk memastikan hasil perhitungan gaya dalam yang diperoleh dari program sesuai dengan perhitungan manual dan memenuhi prinsip keseimbangan statika. Hasil dari program Python akan dibandingkan dengan hasil perhitungan teoritis pada struktur rangka batang.

### A. Validasi Reaksi Tumpuan

Reaksi tumpuan diperiksa menggunakan persamaan keseimbangan gaya vertikal dan momen. Pada model dengan beban 10 kN di tengah bentang, reaksi tumpuan kiri dan kanan seharusnya memiliki nilai yang sama, yaitu 5 kN.

### B. Validasi Gaya Batang

Nilai gaya aksial setiap batang yang diperoleh dari program dibandingkan dengan hasil perhitungan manual menggunakan metode titik simpul. Perbandingan dilakukan untuk memastikan nilai gaya tarik dan tekan pada setiap batang sesuai.

### C. Validasi Keseimbangan

Hasil perhitungan diperiksa berdasarkan persamaan:

ΣF_x = 0

ΣF_y = 0

ΣM = 0

Persamaan tersebut digunakan untuk memastikan struktur berada dalam kondisi seimbang setelah menerima beban.

### D. Analisis Galat

Persentase galat dihitung dengan membandingkan hasil program dengan hasil perhitungan manual menggunakan persamaan:

Error (%) = |Hasil Program - Hasil Manual| / |Hasil Manual| × 100%

Nilai galat yang mendekati 0% menunjukkan bahwa hasil program semakin mendekati hasil perhitungan manual.

---

## 11. Output yang Direncanakan

Output yang direncanakan dari proyek analisis gaya dalam rangka batang adalah:

1. Model struktur rangka batang 2D beserta ukuran dan posisi titik simpul.
2. Visualisasi beban dan jenis tumpuan pada struktur.
3. Hasil perhitungan reaksi tumpuan.
4. Nilai gaya aksial pada setiap batang.
5. Identifikasi batang yang mengalami gaya tarik dan gaya tekan.
6. Visualisasi struktur berdasarkan jenis gaya yang bekerja pada batang.
7. Tabel perbandingan hasil perhitungan manual dan numerik.
8. Nilai persentase galat dari hasil perhitungan.
9. Kesimpulan mengenai distribusi gaya dalam pada struktur rangka batang.

---

## 12. Struktur Repository (Rencana)

Repository GitHub digunakan untuk menyimpan kode program, parameter struktur, dokumentasi, dan hasil analisis agar proyek tersusun dengan baik dan mudah dikembangkan.

### Struktur Folder

Analisis-Gaya-Dalam-Rangka-Batang/

├── README.md

├── PENGERTIAN.md

├── src/

│   ├── perhitungan_reaksi.py

│   ├── perhitungan_gaya_batang.py

│   └── main.py

├── data/

│   └── parameter_struktur.csv

├── hasil/

│   ├── tabel_gaya_batang.csv

│   └── hasil_perhitungan.txt

├── dokumentasi/

│   ├── model_struktur.png

│   └── dokumentasi_proyek.pdf

└── referensi/

    └── sumber_referensi.pdf

### Fungsi Setiap Folder dan File

- README.md: Berisi penjelasan umum proyek, tujuan, dan cara menjalankan program.
- PENGERTIAN.md: Berisi latar belakang, skenario, parameter, asumsi, model matematis, metode numerik, dan validasi proyek.
- src/: Menyimpan kode Python untuk perhitungan reaksi tumpuan, gaya batang, dan program utama.
- data/: Menyimpan data parameter struktur, dimensi, serta beban yang digunakan dalam analisis.
- hasil/: Menyimpan hasil perhitungan berupa tabel gaya batang dan ringkasan hasil program.
- dokumentasi/: Menyimpan gambar struktur, proses pengerjaan, dan dokumentasi proyek.
- referensi/: Menyimpan sumber teori, buku, jurnal, dan referensi yang digunakan dalam proyek.

