# Portofolio Analisis Ekonomi

Repo ini berisi kumpulan analisis ekonomi yang saya kerjakan sebagai mahasiswa
Ekonomi Universitas Brawijaya. Fokus utama: data Indonesia, pendekatan kuantitatif,
dan interpretasi berbasis teori ekonomi.

---

## Struktur folder

```
econ-portfolio/
├── data/
│   ├── raw/          # data asli, tidak dimodifikasi
│   └── processed/    # data yang sudah dibersihkan
├── notebooks/        # analisis utama (Jupyter Notebook)
├── scripts/          # script Python yang bisa dijalankan ulang
├── outputs/
│   ├── figures/      # grafik dan visualisasi
│   └── tables/       # tabel hasil analisis
└── docs/             # catatan metodologi dan referensi
```

---

## 📓 Proyek

| No | Judul | Topik | Tools | Notebook |
|----|-------|-------|-------|----------|
| 01 | Eksplorasi Makroekonomi Indonesia | Tren GDP, inflasi, pengangguran 2000–2022 | pandas, matplotlib | [Buka ↗](https://nbviewer.org/github/ArmandyaDanu/econ-portfolio/blob/main/notebooks/01_eksplorasi_data.ipynb) |
| 02 | Phillips Curve Indonesia | Regresi OLS inflasi vs pengangguran | statsmodels, seaborn | [Buka ↗](https://nbviewer.org/github/ArmandyaDanu/econ-portfolio/blob/main/notebooks/02_phillips_curve_ols.ipynb) |
| 03 | ARIMA Forecasting Inflasi | Time series forecast inflasi 2025 | ARIMA, scikit-learn | [Buka ↗](https://nbviewer.org/github/ArmandyaDanu/econ-portfolio/blob/main/notebooks/03_arima_forecasting_inflasi.ipynb) |
| 04 | DCF Valuation UNVR | Equity research + sensitivity analysis | yfinance, numpy | [Buka ↗](https://nbviewer.org/github/ArmandyaDanu/econ-portfolio/blob/main/notebooks/04_unvr_dcf_valuation.ipynb) |
| 05 | Komparasi Bank Big-3 | Rasio keuangan + valuasi BBCA, BMRI, BBRI | pandas, seaborn | [Buka ↗](https://nbviewer.org/github/ArmandyaDanu/econ-portfolio/blob/main/notebooks/05_banking_comparison.ipynb) |

*Tabel ini akan terus diperbarui seiring bertambahnya analisis.*

---

## Tools yang digunakan

- **Python 3.x** — bahasa utama analisis
- **pandas** — manipulasi dan pembersihan data
- **matplotlib / seaborn** — visualisasi
- **statsmodels** — regresi dan pengujian statistik
- **Jupyter Notebook** — lingkungan analisis interaktif

---

## Cara menjalankan

1. Clone repo ini:
   ```bash
   git clone https://github.com/USERNAME/econ-portfolio.git
   ```
2. Install dependensi:
   ```bash
   pip install pandas matplotlib seaborn statsmodels jupyter
   ```
3. Buka notebook:
   ```bash
   jupyter notebook
   ```

---

## Tentang saya

Mahasiswa Ekonomi Universitas Brawijaya. Aktif di organisasi 180DC UB, BEM, dan
beberapa unit kegiatan mahasiswa lainnya. Tertarik pada analisis data ekonomi,
investasi, dan kebijakan publik.

> *"An economist is someone who sees something work in practice and wonders if it
> works in theory."* — Ronald Reagan
