# Proyek Praktikum SCPK IF-G (093 & 097) - SPK Pemilihan Smartphone

Repositori ini berisi kode sumber untuk aplikasi **Sistem Pendukung Keputusan (SPK)** berbasis antarmuka web interaktif menggunakan **Streamlit**. Aplikasi ini dirancang untuk merekomendasikan smartphone terbaik berdasarkan berbagai kriteria spesifikasi perangkat keras dan harga, dengan menerapkan metode **Weighted Product (WP)**. 

Proyek ini dibuat untuk pemenuhan tugas mata kuliah Praktikum Sistem Cerdas Pendukung Keputusan (SCPK) kelas IF-G.

## 📱 Deskripsi Proyek

Metode *Weighted Product* (WP) digunakan dalam sistem ini untuk memberikan peringkat (ranking) pada berbagai model smartphone yang ada di dalam dataset (`smartphones_clean.csv`). Pengguna dapat menyesuaikan sendiri tingkat kepentingan (bobot) dari setiap kriteria melalui slider yang disediakan di *sidebar* aplikasi, sehingga hasil rekomendasi bisa sangat disesuaikan dengan preferensi masing-masing pengguna.

### Kriteria Keputusan
Sistem ini mengevaluasi smartphone berdasarkan 7 kriteria utama:
1. **Harga** (Atribut: *Cost* - Semakin murah semakin baik)
2. **Rating** (Atribut: *Benefit* - Semakin besar semakin baik)
3. **Prosesor** (Atribut: *Benefit* - Semakin cepat/besar semakin baik)
4. **RAM** (Atribut: *Benefit* - Semakin besar semakin baik)
5. **Storage / Penyimpanan** (Atribut: *Benefit* - Semakin besar semakin baik)
6. **Kamera** (Atribut: *Benefit* - Semakin besar resolusi semakin baik)
7. **Baterai** (Atribut: *Benefit* - Semakin besar kapasitas semakin baik)

## 🚀 Fitur Aplikasi (Navigasi Halaman)

Aplikasi ini dibagi menjadi 4 halaman utama untuk memudahkan pemahaman proses SPK dari awal hingga akhir:

- **Page 1 - Data Alternatif:** Menampilkan dataset mentah smartphone yang digunakan, serta rincian tipe atribut (Cost/Benefit) untuk masing-masing kriteria.
- **Page 2 - Penjelasan WP:** Halaman edukasi yang berisi pengertian, tujuan, rumus normalisasi bobot, serta langkah-langkah perhitungan matematika untuk Vektor S dan Vektor V dalam metode Weighted Product.
- **Page 3 - Perhitungan WP:** Menampilkan secara transparan proses perhitungan, mulai dari matriks keputusan awal, hasil normalisasi bobot, hingga tabel peringkat (Top 10) dan pengumuman smartphone pemenang.
- **Page 4 - Visualisasi:** Menyajikan grafik interaktif berupa:
  - *Pie Chart* untuk persentase proporsi bobot kriteria yang diatur pengguna.
  - *Bar Chart* untuk Top 10 Ranking Smartphone.
  - Grafik profil nilai kriteria dari smartphone pemenang.

## 🛠️ Prasyarat & Instalasi

Untuk menjalankan aplikasi ini secara lokal, pastikan Anda telah menginstal Python di komputer Anda. Anda juga memerlukan beberapa pustaka Python berikut:
- `streamlit`
- `pandas`
- `numpy`
- `matplotlib`

### Cara Menjalankan Aplikasi

1. Clone repositori ini ke komputer lokal Anda:
   ```bash
   git clone <url-repositori-anda>
   cd Proyek_PrakSCPK_IFG_093_097
