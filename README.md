# Studi Ablasi RNN, LSTM, GRU vs ANN untuk Prediksi Trafik Seluler Milan

Tugas Workshop Deep Learning — Teknik Telekomunikasi ITERA.

<!-- Ganti seluruh isian bertanda [ ... ] di bawah. Hapus komentar ini. -->

## Kelompok

| Peran | Nama | NIM |
|---|---|---|
| Ketua | [Angelina Gultom] | [124400072] |
| Anggota | [Trisna Anggraeni Gea] | [124400043] |
| Anggota | [Amelda Wulandari] | [124400090] |

- **Kelas:** [RB]
- **Lokasi kelompok:** [0] — [Stazione Centrale] (0)
- **Laporan:** [`laporan-latex/main.pdf`]

## Cara Menjalankan

```bash
uv sync
uv run jupyter lab
```

Buka `tugas_ablasi.ipynb`, isi `LOKASI_KELOMPOK`, lalu jalankan semua sel. Semua run tercatat di `hasil/ablasi.csv`.

Perangkat yang kami pakai: ASUS Vivobook Go E1404FA (AMD Ryzen 3 7320U) dan Axioo Hype 5 AMD, Total waktu training rata-rata: 15 menit.
## Ringkasan Hasil

[ Model GRU dan RNN memberikan performa test MAE terbaik pada panjang jendela waktu $W = 48$ jam, dengan kestabilan konvergensi yang lebih baik dibandingkan ANN.]

## Struktur

```
tugas_ablasi.ipynb      notebook eksperimen (di-commit beserta output)
data/                   Berisi dataset trafik seluler Milano
hasil/                  Berisi grafik hasil eksperimen ablasi dan grafik kovergensi
laporan-latex/          File sumber LaTeX untuk penyusunan laporan format IEEE
starter/                Skrip utama pelatihan dan evaluasi model
```

## Data

Telecom Italia Big Data Challenge (Barlacchi dkk., 2015, *Scientific Data*, lisensi ODbL), versi per jam dari Zhang dkk. (INFOCOM 2021). Disiapkan oleh pengajar di repo [mctosima/dl-workshop](https://github.com/mctosima/dl-workshop).
