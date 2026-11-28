
# ANALISIS GAYA DALAM PADA STRUKTUR RANGKA BATANG MENGGUNAKAN PERHITUNGAN NUMERIK

## 1. Latar Masalah

Struktur rangka batang merupakan salah satu bentuk struktur yang banyak digunakan dalam konstruksi teknik sipil, seperti jembatan, rangka atap, dan struktur bangunan. Setiap batang pada struktur memiliki peran dalam menyalurkan beban yang bekerja menuju tumpuan.

Ketika suatu struktur menerima beban, setiap batang dapat mengalami gaya tarik atau gaya tekan yang berbeda, tergantung pada bentuk struktur, posisi beban, dan kondisi tumpuannya. Jika gaya yang terjadi tidak dianalisis dengan baik, maka dapat menyebabkan kesalahan dalam memahami perilaku struktur.

Proyek ini berfokus pada analisis gaya dalam pada struktur rangka batang sederhana menggunakan perhitungan numerik. Perhitungan dilakukan untuk mengetahui besarnya gaya aksial pada setiap batang, mengidentifikasi batang yang mengalami tarik dan tekan, serta membandingkan hasil perhitungan program dengan perhitungan teoritis. Dengan demikian, perhitungan numerik dapat membantu memahami distribusi gaya pada struktur secara lebih sistematis.

---

## 2. Jenis-Jenis Pembebanan

### A. Beban Terpusat (Point Load)

Beban yang bekerja pada satu titik tertentu pada struktur, misalnya beban yang diberikan pada titik sambungan rangka atau beban kendaraan pada bagian tertentu jembatan.

### B. Beban Terbagi Merata (Uniformly Distributed Load)

Beban yang tersebar secara merata sepanjang struktur, misalnya berat material atap yang diteruskan ke rangka.

### C. Beban Segitiga

Beban yang besarannya berubah secara bertahap sepanjang struktur, misalnya distribusi beban yang meningkat dari satu ujung ke ujung lainnya.

### D. Beban Kombinasi

Gabungan dari beberapa jenis beban yang bekerja secara bersamaan, seperti beban mati dan beban hidup pada struktur bangunan.

Pada proyek ini, pembebanan utama yang digunakan adalah beban terpusat pada titik simpul bagian atas rangka batang agar analisis gaya pada setiap batang lebih mudah dilakukan.

---

## 3. Jenis-Jenis Tumpuan

### A. Tumpuan Sendi (Pin Support)

Tumpuan yang menahan perpindahan horizontal dan vertikal, tetapi memungkinkan struktur berotasi.

### B. Tumpuan Rol (Roller Support)

Tumpuan yang menahan perpindahan vertikal, tetapi memungkinkan perpindahan horizontal dan rotasi.

### C. Tumpuan Jepit (Fixed Support)

Tumpuan yang menahan perpindahan horizontal, vertikal, dan rotasi sehingga ujung struktur tidak dapat bergerak maupun berputar.

Pada proyek ini digunakan kombinasi tumpuan sendi dan rol karena merupakan sistem tumpuan sederhana yang umum digunakan pada struktur serta memudahkan penentuan reaksi tumpuan.

---

## 4. Alasan Memilih Gaya Dalam

Gaya dalam dipilih karena merupakan bagian penting dalam analisis struktur teknik sipil untuk mengetahui bagaimana suatu struktur merespons beban yang bekerja.

Melalui analisis gaya dalam, dapat diketahui batang mana yang mengalami tarik dan batang mana yang mengalami tekan. Hal ini membantu memahami bagaimana beban diteruskan melalui struktur hingga mencapai tumpuan.

Selain itu, perhitungan gaya dalam dapat dikembangkan menggunakan perhitungan numerik sehingga perhitungan tidak hanya dilakukan secara manual, tetapi juga dapat diselesaikan menggunakan program komputer. Topik ini dipilih karena memiliki penerapan langsung pada struktur nyata dan dapat menunjukkan hubungan antara matematika serta bidang teknik sipil.

---

## 5. Skenario

| Item | Pilihan | Justifikasi |
|---|---|---|
| Struktur | Rangka batang segitiga 2D | Bentuk sederhana dan stabil untuk analisis awal |
| Tumpuan | Sendi di A dan rol di B | Memudahkan perhitungan reaksi tumpuan |
| Pembebanan | Beban vertikal terpusat di titik C | Menunjukkan distribusi gaya pada batang |
| Material | Baja | Material yang umum digunakan pada rangka batang |
| Fokus analisis | Gaya aksial batang | Untuk mengetahui gaya tarik dan tekan |
| Metode | Perhitungan numerik berbasis persamaan statika | Memudahkan perhitungan gaya secara sistematis |

Skenario yang digunakan adalah rangka batang segitiga dengan dua tumpuan di bagian bawah dan satu titik simpul di bagian atas. Struktur menerima beban vertikal pada titik atas, kemudian gaya didistribusikan melalui ketiga batang menuju tumpuan.

---

## 6. Parameter dan Justifikasi

| Parameter | Simbol | Nilai | Justifikasi |
|---|---|---:|---|
| Panjang bentang | L | 8 m | Bentang model rangka sederhana |
| Tinggi rangka | h | 3 m | Membentuk geometri segitiga |
| Beban vertikal | P | 10 kN | Beban terpusat untuk simulasi |
| Modulus elastisitas | E | 200 GPa | Nilai pendekatan material baja |
| Luas penampang batang | A | 1.000 mm² | Penampang seragam untuk model awal |
| Jumlah titik simpul | n | 3 | Dua titik tumpuan dan satu titik beban |
| Jumlah batang | m | 3 | Membentuk rangka batang segitiga |
| Jenis struktur | - | Rangka batang 2D | Mempermudah analisis matematis |

Nilai parameter di atas merupakan nilai asumsi untuk model proyek dan bukan ukuran struktur bangunan yang sudah dirancang untuk digunakan di lapangan.

---

## 7. Asumsi Model

Dalam analisis ini, beberapa asumsi digunakan agar model lebih sederhana dan perhitungan dapat dilakukan, yaitu:

1. Struktur berbentuk rangka batang segitiga dalam bidang dua dimensi.
2. Setiap batang memiliki bentuk lurus.
3. Sambungan antarbatang dianggap berupa sendi.
4. Beban bekerja pada titik simpul.
5. Setiap batang hanya menerima gaya aksial, yaitu tarik atau tekan.
6. Material baja dianggap homogen.
7. Luas penampang seluruh batang dianggap sama.
8. Struktur berada dalam kondisi stabil.
9. Perubahan bentuk struktur dianggap kecil.
10. Berat sendiri batang diabaikan.
11. Beban yang bekerja bersifat statis dan tidak berubah terhadap waktu.

---

## 8. Model Matematis

Model matematis menggunakan prinsip keseimbangan statika untuk menentukan reaksi tumpuan dan gaya aksial pada setiap batang rangka. Perhitungan dilakukan berdasarkan keseimbangan gaya horizontal, gaya vertikal, dan momen.

### 8.1 Geometri Struktur

Diketahui:

- Panjang bentang = 8 m
- Tinggi rangka = 3 m
- Beban terpusat P = 10 kN
- Tumpuan A = sendi
- Tumpuan B = rol
- Titik C = titik beban di puncak

Panjang batang miring:

L_AC = √(4² + 3²)

L_AC = √(16 + 9)

L_AC = √25

L_AC = 5 m

Karena struktur simetris:

L_BC = 5 m

Sudut batang miring:

sin θ = 3/5 = 0,6

cos θ = 4/5 = 0,8

### 8.2 Perhitungan Reaksi Tumpuan

Karena beban berada tepat di tengah bentang dan struktur simetris, reaksi tumpuan kiri dan kanan sama besar.

Diketahui:

P = 10 kN

L = 8 m

Momen terhadap titik A:

ΣM_A = 0

R_B × 8 - 10 × 4 = 0

8R_B = 40

R_B = 40/8

R_B = 5 kN

Keseimbangan gaya vertikal:

ΣF_y = 0

R_A + R_B - P = 0

R_A + 5 - 10 = 0

R_A = 5 kN

Jadi, reaksi pada kedua tumpuan adalah 5 kN ke atas.

### 8.3 Perhitungan Gaya Batang Miring

Dari geometri struktur:

sin θ = 3/5

Pada titik C, terdapat dua batang miring yang menahan beban vertikal 10 kN.

Keseimbangan gaya vertikal:

ΣF_y = 0

2F sin θ - 10 = 0

2F(3/5) = 10

(6/5)F = 10

F = 10 × 5/6

F = 8,33 kN

Kedua batang miring AC dan BC mengalami gaya sebesar 8,33 kN tekan.

### 8.4 Perhitungan Gaya Batang Horizontal

Diketahui:

cos θ = 4/5

Keseimbangan gaya horizontal pada titik A:

ΣF_x = 0

F_AB - F_AC cos θ = 0

F_AB = 8,33 × (4/5)

F_AB = 6,664 kN

F_AB ≈ 6,67 kN

Batang AB mengalami gaya tarik.

### 8.5 Hasil Perhitungan Gaya Dalam

| Nama Batang | Gaya Aksial | Jenis Gaya |
|---|---:|---|
| AC | 8,33 kN | Tekan |
| BC | 8,33 kN | Tekan |
| AB | 6,67 kN | Tarik |

### 8.6 Persamaan yang Digunakan

Persamaan keseimbangan yang menjadi dasar perhitungan:

ΣF_x = 0

ΣF_y = 0

ΣM = 0

Gaya aksial batang ditentukan melalui keseimbangan gaya pada masing-masing titik simpul. Untuk batang miring, gaya diuraikan menjadi komponen horizontal dan vertikal menggunakan trigonometri:

F_x = F cos θ

F_y = F sin θ

Hasil perhitungan manual tersebut menjadi nilai pembanding untuk hasil program numerik.

---

## 9. Rencana Metode Numerik

Metode yang digunakan adalah perhitungan numerik berbasis persamaan statika dan trigonometri yang diterapkan ke dalam program Python.

| Metode | Fungsi dalam Proyek | Alasan |
|---|---|---|
| Perhitungan reaksi tumpuan | Menentukan gaya pada tumpuan A dan B | Memastikan struktur seimbang |
| Perhitungan trigonometri | Menentukan komponen gaya pada batang miring | Mengetahui gaya horizontal dan vertikal |
| Perhitungan gaya aksial | Menentukan gaya tarik dan tekan pada batang | Mengetahui kondisi setiap batang |
| Python | Mengotomatisasi perhitungan | Mengurangi kesalahan hitung dan mempercepat proses |

### Tahapan Perhitungan Program

1. Memasukkan parameter geometri struktur.
2. Memasukkan nilai beban.
3. Menghitung panjang batang miring.
4. Menghitung nilai sin dan cos sudut batang.
5. Menghitung reaksi tumpuan.
6. Menghitung gaya batang miring.
7. Menghitung gaya batang horizontal.
8. Menentukan jenis gaya pada setiap batang.
9. Membandingkan hasil program dengan perhitungan manual.
10. Menampilkan hasil dalam tabel.

Metode ini digunakan untuk menerapkan perhitungan matematis ke dalam program sehingga hasil dapat diperoleh secara otomatis dan konsisten.

---

## 10. Rencana Validasi

Validasi dilakukan untuk memastikan hasil perhitungan program sesuai dengan prinsip keseimbangan struktur dan menghasiln dengan perhitungan manual menggunakan persamaan keseimbangan statika:

ΣF_x = 0

ΣF_y = 0

ΣM = 0

Perhitungan manual digunakan sebagai nilai acuan untuk mengetahui gaya yang bekerja pada setiap batang.

### B. Validasi Keseimbangan Struktur

Memeriksa apakah struktur memenuhi keseimbangan gaya horizontal, gaya vertikal, dan momen.

### C. Validasi Gaya Batang

Membandingkan nilai gaya aksial hasil program dengan hasil perhitungan manual melalui metode titik simpul.

### D. Analisis Galat

Persentase galat dihitung menggunakan persamaan:

Error (%) = |Hasil Program - Hasil Manual| / |Hasil Manual| × 100%

Keterangan:

- Hasil Program = hasil perhitungan menggunakan Python
- Hasil Manual = hasil perhitungan teoritis

Jika hasil keduanya mendekati sama, maka program dianggap memberikan hasil yang sesuai dengan perhitungan teoritis pada model tersebut.

---

## 11. Output yang Direncanakan

Output yang diharapkan dari proyek ini adalah:

1. Gambar model struktur rangka batang 2D.
2. Gambar posisi beban dan jenis tumpuan.
3. Koordinat setiap titik simpul.
4. Nilai reaksi tumpuan.
5. Nilai gaya aksial pada setiap batang.
6. Identifikasi batang yang mengalami tarik dan tekan.
7. Diagram gaya pada struktur.
8. Tabel perbandingan hasil perhitungan manual dan program.
9. Nilai persentase galat.
10. Kesimpulan mengenai hasil analisis gaya dalam.

---

## 12. Struktur Repository (Rencana)

Struktur repository GitHub direncanakan untuk memisahkan dokumen, kode program, data parameter, dan hasil analisis agar pengerjaan proyek lebih terorganisir.

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

│   └── laporan.pdf

└── referensi/

    └── jurnal_dan_sumber.pdf

### Fungsi Folder

- README.md : berisi penjelasan proyek, tujuan, dan cara menjalankan program.
- PENGERTIAN.md : berisi latar belakang dan penjelasan analisis proyek dari nomor 1 sampai 12.
- src/ : tempat menyimpan kode program perhitungan.
- data/ : tempat menyimpan parameter struktur dan pembebanan.
- hasil/ : tempat menyimpan tabel serta hasil perhitungan program.
- dokumentasi/ : tempat menyimpan gambar model dan laporan proyek.
- referensi/ : tempat menyimpan jurnal serta sumber pendukung.

---

## 13. Referensi

1. Hibbeler, R. C. Structural Analysis. Pearson. (Materi analisis struktur, reaksi tumpuan, dan gaya dalam).
2. Kassimali, A. Structural Analysis. Cengage Learning. (Materi analisis rangka batang dan keseimbangan struktur).
3. Logan, D. L. A First Course in the Finite Element Method. Cengage Learning. (Materi dasar metode numerik dan analisis struktur).
4. Chapra, S. C., & Canale, R. P. Numerical Methods for Engineers. McGraw-Hill. (Materi penyelesaian persamaan numerik).
5. Re

