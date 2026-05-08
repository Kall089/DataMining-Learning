# 📊 Day 2: Mean, Median, Mode — Kapan Masing-Masing Misleading

**Bulan**: 1 — Foundation | **Minggu**: 1 — Data & Statistik Dasar  
**Estimasi Waktu**: 2–3 jam teori + 3–4 jam latihan = **5–7 jam total**

---

## 🎯 Learning Objectives

Setelah menyelesaikan Day 2, kamu akan:
- [ ] Menghitung mean, median, mode secara manual dan dengan Python
- [ ] Menjelaskan kapan mean **menipu** (misleading) dan mengapa
- [ ] Memahami konsep **resistant statistics** (robust terhadap outlier)
- [ ] Menggunakan trimmed mean sebagai alternatif yang lebih robust
- [ ] Menghitung dan menginterpretasi weighted mean
- [ ] Memilih ukuran tendensi sentral yang **tepat** berdasarkan distribusi data
- [ ] Mendeteksi kapan mean ≠ median menunjukkan skewness
- [ ] Mengaplikasikan konsep ke real-world cases (gaji, harga properti, dll.)

---

## 📋 Prerequisites

- **Day 1**: Tipe data, Pandas DataFrame, `.describe()`
- Python dasar: list, loop, function
- Library: `numpy`, `pandas`, `matplotlib`, `seaborn`, `scipy`

```bash
pip install numpy pandas matplotlib seaborn scipy
```

---

## 📁 Struktur Folder

```
Day-02 (Mean, Median, Mode)/
├── teori/
│   └── Day_02_Teori_Lengkap.ipynb    ← Mulai di sini!
├── latihan/
│   ├── exercise_1.ipynb    # Hitung & bandingkan mean vs median (Easy)
│   ├── exercise_2.ipynb    # Deteksi outlier dengan mean-median gap (Easy)
│   ├── exercise_3.ipynb    # Trimmed mean & weighted mean (Medium)
│   ├── exercise_4.ipynb    # Analisis distribusi gaji (Medium)
│   └── exercise_5.ipynb    # Studi kasus harga properti (Medium-Hard)
├── solusi/
│   ├── solution_1.ipynb    ← Lihat SETELAH mencoba sendiri!
│   ├── solution_2.ipynb
│   ├── solution_3.ipynb
│   ├── solution_4.ipynb
│   └── solution_5.ipynb
├── tugas/                   ← 15 soal TANPA solusi!
│   ├── tugas_01.ipynb       # Mean dari list (Easy)
│   ├── tugas_02.ipynb       # Median dari list (Easy)
│   ├── tugas_03.ipynb       # Mode dari list (Easy)
│   ├── tugas_04.ipynb       # Mean vs Median comparison (Easy)
│   ├── tugas_05.ipynb       # Efek outlier pada mean (Easy)
│   ├── tugas_06.ipynb       # Trimmed mean (Medium)
│   ├── tugas_07.ipynb       # Weighted mean IPK (Medium)
│   ├── tugas_08.ipynb       # Identifikasi skewness (Medium)
│   ├── tugas_09.ipynb       # Multi-modal data (Medium)
│   ├── tugas_10.ipynb       # Real-world: pendapatan daerah (Medium)
│   ├── tugas_11.ipynb       # Grouped statistics (Hard)
│   ├── tugas_12.ipynb       # Robust statistics comparison (Hard)
│   ├── tugas_13.ipynb       # Simulasi sampling (Hard)
│   ├── tugas_14.ipynb       # Analisis distribusi bimodal (Hard)
│   └── tugas_15.ipynb       # Comprehensive case study (Hard)
└── README.md               ← File ini
```

---

## 🗺️ Step-by-Step Learning Guide

### Step 1: Baca Teori (60–90 menit)
1. Buka `teori/Day_02_Teori_Lengkap.ipynb`
2. Jalankan setiap cell dari atas ke bawah (**Run All** atau Shift+Enter)
3. Fokus pada:
   - Definisi dan intuisi mean, median, mode
   - Kapan mean menipu (contoh real-world)
   - Konsep resistant statistics
   - Trimmed mean dan weighted mean
   - Hubungan mean-median-skewness

### Step 2: Latihan (3–4 jam)

| Exercise | Topik | Estimasi | Priority |
|----------|-------|----------|----------|
| `exercise_1.ipynb` | Hitung & bandingkan mean vs median | 30 mnt | ⭐⭐⭐ Wajib |
| `exercise_2.ipynb` | Deteksi outlier dengan mean-median gap | 40 mnt | ⭐⭐⭐ Wajib |
| `exercise_3.ipynb` | Trimmed mean & weighted mean | 45 mnt | ⭐⭐⭐ Wajib |
| `exercise_4.ipynb` | Analisis distribusi gaji perusahaan | 45 mnt | ⭐⭐ Penting |
| `exercise_5.ipynb` | Studi kasus harga properti | 60 mnt | ⭐⭐⭐ Wajib |

### Step 3: Review Solusi (30 menit)
- Buka solusi HANYA setelah mencoba sendiri minimal 15 menit
- Bandingkan pendekatan kamu dengan solusi
- Catat teknik yang belum kamu gunakan

### Step 4: Kerjakan Tugas (2–3 jam)

Folder `tugas/` berisi **15 soal tanpa solusi** — kerjakan mandiri!

| Tugas | Topik | Difficulty |
|-------|-------|------------|
| `tugas_01` - `tugas_05` | Hitung mean/median/mode, efek outlier | Easy |
| `tugas_06` - `tugas_10` | Trimmed/weighted mean, skewness, real-world | Medium |
| `tugas_11` - `tugas_15` | Grouped stats, robust comparison, simulasi | Hard |

> **Format**: Setiap notebook berisi soal + data input + expected output. Kamu hanya perlu mengisi cell `# TODO`.

---

## 📦 Dataset yang Digunakan

| Notebook | Dataset | Cara Load |
|----------|---------|-----------|
| Teori | Gaji perusahaan sintetis | `np.random` dengan seed=42 |
| Teori | Tips (Seaborn) | `sns.load_dataset('tips')` |
| exercise_1 | Nilai ujian sintetis | Sudah di-generate di notebook |
| exercise_2 | Data penjualan sintetis | Sudah di-generate di notebook |
| exercise_3 | Data mahasiswa sintetis | Sudah di-generate di notebook |
| exercise_4 | Data gaji perusahaan | Sudah di-generate di notebook |
| exercise_5 | Data harga properti | Sudah di-generate di notebook |

> Semua dataset sudah tersedia di dalam notebook — tidak perlu download eksternal.

---

## ✅ Checklist Sebelum Lanjut ke Day 3

### Konsep
- [ ] Bisa menjelaskan perbedaan mean, median, mode dalam 1 kalimat masing-masing
- [ ] Tahu kapan mean menipu dan bisa memberi 3 contoh real-world
- [ ] Paham mengapa median disebut "resistant statistic"
- [ ] Bisa menjelaskan hubungan mean > median → right-skewed
- [ ] Tahu kapan pakai trimmed mean vs median vs mean

### Teknik Python
- [ ] Bisa hitung mean, median, mode dengan NumPy/Pandas/SciPy
- [ ] Bisa hitung trimmed mean dengan `scipy.stats.trim_mean()`
- [ ] Bisa hitung weighted mean dengan `np.average(weights=...)`
- [ ] Bisa visualisasi distribusi + garis mean/median dalam satu plot
- [ ] Bisa gunakan `.skew()` untuk mengukur skewness

### Exercise
- [ ] Selesaikan minimal **4 dari 5 exercise**
- [ ] Bisa jawab pertanyaan refleksi di setiap exercise

### Tugas
- [ ] Selesaikan minimal **10 dari 15 tugas**
- [ ] Output yang dihasilkan sesuai dengan expected output
- [ ] Tugas 1-5 (Easy) wajib semua benar

---

## 🔑 Quick Reference — Fungsi Statistik Day 2

```python
import numpy as np
import pandas as pd
from scipy import stats

# === MEAN ===
np.mean(data)                    # Mean NumPy
df['kolom'].mean()               # Mean Pandas
np.average(data, weights=w)      # Weighted mean

# === MEDIAN ===
np.median(data)                  # Median NumPy
df['kolom'].median()             # Median Pandas

# === MODE ===
stats.mode(data)                 # Mode SciPy (returns array)
df['kolom'].mode()               # Mode Pandas (bisa > 1 nilai)

# === TRIMMED MEAN ===
stats.trim_mean(data, 0.1)      # Trim 10% dari kedua ujung

# === SKEWNESS ===
df['kolom'].skew()               # > 0 = right-skewed, < 0 = left-skewed

# === QUICK COMPARISON ===
print(f"Mean:   {df['kolom'].mean():.2f}")
print(f"Median: {df['kolom'].median():.2f}")
print(f"Mode:   {df['kolom'].mode()[0]:.2f}")
print(f"Skew:   {df['kolom'].skew():.4f}")
```

---

## ⚠️ Common Mistakes Day 2

1. **Selalu pakai mean** — SALAH! Mean sangat sensitif terhadap outlier. Cek distribusi dulu!
2. **Median untuk semua** — SALAH! Median membuang informasi. Jika data simetris, mean lebih informatif
3. **Mode = "rata-rata"** — SALAH! Mode adalah nilai **paling sering muncul**, bukan rata-rata
4. **Lupa cek distribusi** — Selalu plot histogram SEBELUM memilih ukuran central tendency
5. **Trimmed mean = median** — SALAH! Trimmed mean masih menghitung rata-rata, hanya menghilangkan extreme values
6. **Weighted mean tanpa normalisasi bobot** — Bobot tidak harus berjumlah 1, tapi harus konsisten

---

## 🔮 Preview Day 3

**Day 3: Variance, Standard Deviation, IQR — Mengukur Spread Data**

Topics yang akan dipelajari:
- Variance: rata-rata jarak kuadrat dari mean
- Standard deviation: akar dari variance, satuan sama dengan data
- IQR (Interquartile Range): Q3 - Q1, robust terhadap outlier
- Range vs IQR vs Std — kapan pakai mana
- Coefficient of Variation: membandingkan spread antar dataset berbeda

**Preparation**: Pastikan sudah paham mean dan median dari Day 2!

---

## 📈 Progress Tracking

- Date: _____________
- Exercise selesai: ____ / 5
- Tugas selesai: ____ / 15
- Waktu total: ____ jam
- Konsep yang masih bingung:
  ```

  ```

---

*"Mean bisa menipu, median bisa menyembunyikan informasi, mode bisa tidak ada. Seorang data miner yang baik tahu kapan pakai yang mana."* 🎯
