# WILKERSTAT 6500 — Kalimantan Utara

Peta web interaktif untuk menjelajahi wilayah kerja statistik (Wilkerstat) Provinsi
Kalimantan Utara, dari level kabupaten/kota, kecamatan, desa/kelurahan, hingga SLS
(Satuan Lingkungan Setempat / RT/RW/Dusun), dengan basemap citra satelit.

Wilkerstat (wilayah kerja statistik) adalah kerangka kerja yang digunakan Badan
Pusat Statistik (BPS) untuk melaksanakan sensus dan survei. Wilkerstat menyediakan
batas wilayah geografis yang dipakai untuk mengorganisasi dan mengidentifikasi
wilayah kerja statistik, yang diperbarui setiap tahun.

## Akses

Aplikasi dapat langsung diakses lewat link berikut:

**[WILKERSTAT 6500](https://abbashalomradja.github.io/wilkerstat-6500/)**

Tidak perlu instalasi apa pun. Cukup buka link di browser (desktop atau mobile).

## Fitur

- Basemap satelit / hybrid / peta jalan — bisa diganti-ganti
- Layer batas kabupaten/kota, kecamatan, desa/kelurahan, dan SLS — bisa
  dinyalakan/dimatikan sendiri-sendiri
- Layer desa otomatis muncul saat peta di-zoom masuk, layer SLS otomatis muncul
  saat zoom lebih dekat lagi, supaya tampilan tetap ringan dilihat
- Data SLS dimuat per kabupaten saat dibutuhkan (bukan sekaligus di awal), agar
  halaman tetap cepat diakses meski jumlah SLS sangat banyak
- Pencarian nama wilayah (kab/kota, kecamatan, desa, SLS) dengan hasil langsung
  di-zoom
- Navigasi berjenjang: pilih kab/kota → kecamatan → desa → SLS lewat dropdown
- Klik wilayah di peta untuk melihat kode wilkerstat lengkap di panel info
- Deteksi lokasi GPS: menampilkan wilayah tempat pengguna berada, sampai level
  SLS bila datanya sudah termuat

## Cakupan data

| Level          | Jumlah wilayah |
| -------------- | -------------- |
| Kab/Kota       | 5              |
| Kecamatan      | 55             |
| Desa/Kelurahan | 484            |
| SLS            | 3.157          |

Kode wilayah mengikuti standar BPS (kode provinsi 65 untuk Kalimantan Utara).

## Struktur proyek

```
index.html           halaman utama (peta + data kab/kota, kecamatan, desa)
data/
  sls_01.geojson      data SLS Kabupaten Malinau
  sls_02.geojson      data SLS Kabupaten Bulungan
  sls_03.geojson      data SLS Kabupaten Tana Tidung
  sls_04.geojson      data SLS Kabupaten Nunukan
  sls_71.geojson      data SLS Kota Tarakan
```

> Catatan: karena data SLS dimuat lewat `fetch()` dari folder `data/`, situs ini
> perlu diakses lewat server (mis. GitHub Pages, Live Server) — tidak bisa lagi
> dibuka langsung dengan dobel-klik file `index.html` dari File Explorer.

## Kontak

Ada pertanyaan atau masukan soal proyek ini? Silakan hubungi lewat GitHub.

## Lisensi

Kode pada proyek ini dirilis di bawah [MIT License](https://github.com/AbbashalomRadja/wilkerstat-6500/blob/main/LICENSE). Data batas wilayah
bersumber dari data resmi BPS dan tunduk pada ketentuan penggunaan data BPS.
