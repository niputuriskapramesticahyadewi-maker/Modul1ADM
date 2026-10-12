# Proyek Akuisisi dan Manajemen Data
Mata kuliah : BIFP-243 Akuisisi dan Manajemen Data
Nama / NIM  : Ni Putu Riska Pramesti Cahya Dewi / 2501010315
Tujuan      : Memahami konsep Data Akuisisi dan Manajemen Data

## Struktur Folder 
- data/raw        : data mentah hasil akuisisi (READ-ONLY)
- data/interim    : hasil antara (cleaning, transformasi)
- data/processed  : dataset final siap analisis
- notebooks       : notebook praktikum
- src             : script Python yang dapat digunakan ulang
- docs            : data dictionary dan metadata
- reports         : laporan kualitas data

## Cara Menjalankan Ulang
1. pip install -r requirements.txt
2. Jalankan notebook di folder notebooks secara berurutan

## Contoh Kasus Nyata
Pentingnya Reproducibility dalam Akuisisi Data

Reproducibility (keterulangan) merupakan prinsip krusial dalam akuisisi data untuk menjamin bahwa seluruh proses pengumpulan data dapat diuji, diverifikasi, dan dijalankan ulang oleh pihak lain dengan menghasilkan output yang konsisten. Tanpa reproducibility, pipeline data rentan terhadap bias, kehilangan konteks historis, dan sulit dilacak saat terjadi kesalahan sistem.

Contoh kasus nyata dampak buruk diabaikannya prinsip ini terjadi pada skandal analisis ekonomi Reinhart-Rogoff (2013). Kebijakan ekonomi global yang diterapkan berbagai negara ternyata didasarkan pada riset yang tidak reproducible akibat kesalahan pemrosesan data spreadsheet dan dokumentasi data mentah yang buruk. Ketika peneliti lain mencoba mereplikasi hasil tersebut, ditemukan galat fatal pada formula dan pengelompokan data yang mengubah total kesimpulan riset.

Oleh karena itu, penerapan praktik standar seperti penyimpanan data mentah yang bersifat read-only di folder data/raw, penggunaan version control (Git), serta dokumentasi lingkungan kerja (environment) dan script yang terstruktur sangat vital. Langkah-langkah ini memastikan transparansi, integritas data, serta validitas keputusan berbasis data di tingkat industri maupun akademis.
