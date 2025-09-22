# MBG Food Poisoning Cases (Indonesia, 2025)

Dataset ini berisi kurasi data **kasus keracunan makanan program MBG (Makan Bergizi Gratis)** di Indonesia tahun 2025.

## 📊 Data
- `data/kasus-mbg-clean.csv`  
  Data hasil kurasi dengan kolom:
  - `wilayah` → 1,2,3 sesuai laporan
  - `tanggal_kasus` → format YYYY-MM-DD
  - `provinsi` → sesuai standar 38 provinsi Indonesia
  - `jumlah_kasus` → jumlah orang
  - `update_date` → tanggal update berita (2025-09-22)

## 📖 Sumber Data

- Tempo: [Data BGN Catat Korban Kasus Keracunan MBG Mencapai 4.711 Orang](https://www.tempo.co/politik/data-bgn-catat-korban-kasus-keracunan-mbg-mencapai-4-711-orang-2072315)  
- Liputan6: [Ada 4.711 Korban Kasus Keracunan MBG](https://www.liputan6.com/news/read/6165915/ada-4711-korban-kejadian-luar-biasa-di-mbg-ini-daftar-lengkapnya)  
- Tirto: [9 Bulan Berjalan, BGN Catat 4711 Orang Keracunan MBG](https://tirto.id/9-bulan-berjalan-bgn-catat-4711-orang-keracunan-mbg-hiak)

## 🚀 Cara Pakai

Panggil data langsung dari raw GitHub:

### Via R
```r
url <- "https://raw.githubusercontent.com/wsuryaningrat/mbg-food-poisoning-data/refs/heads/main/data/mbg-data.csv"
df <- read.csv(url,sep = ";")
```

### Via Python
```py
# Python
import pandas as pd
url <- "https://raw.githubusercontent.com/wsuryaningrat/mbg-food-poisoning-data/refs/heads/main/data/mbg-data.csv"
df = pd.read_csv(url,index_col=0,parse_dates=[0])
```
