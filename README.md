# WILKERSTAT 6500 — Kalimantan Utara

Peta web interaktif untuk menjelajahi wilayah kerja statistik (Wilkerstat) Provinsi
Kalimantan Utara, dari level kabupaten/kota, kecamatan, sampai desa/kelurahan,
dengan basemap citra satelit.

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
- Layer batas kabupaten/kota, kecamatan, dan desa/kelurahan — bisa dinyalakan/dimatikan sendiri-sendiri
- Layer desa otomatis muncul saat peta di-zoom masuk, supaya tampilan tetap ringan dilihat
- Pencarian nama wilayah (kab/kota, kecamatan, desa) dengan hasil langsung di-zoom
- Navigasi berjenjang: pilih kab/kota → kecamatan → desa lewat dropdown
- Klik wilayah di peta untuk melihat kode wilkerstat lengkap di panel info
- Satu file HTML saja — data GeoJSON sudah ter-embed di dalamnya, tidak perlu server

## Cakupan data

| Level          | Jumlah wilayah |
|----------------|----------------|
| Kab/Kota       | 5              |
| Kecamatan      | 55             |
| Desa/Kelurahan | 484            |

Kode wilayah mengikuti standar BPS (kode provinsi 65 untuk Kalimantan Utara).

## Kontak

Ada pertanyaan atau masukan soal proyek ini? Silakan hubungi lewat GitHub.

## Lisensi

Kode pada proyek ini dirilis di bawah [MIT License](LICENSE). Data batas wilayah
bersumber dari data resmi BPS dan tunduk pada ketentuan penggunaan data BPS.
