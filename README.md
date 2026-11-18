# Netflix Shows & Movies Exploratory Data Analysis (Python & Pandas)

👤 **Penyusun:** Shafwan Mumtaz  
📊 **Tools:** Python (`pandas`, `numpy`, `matplotlib`, `seaborn`), Jupyter Notebook

---

## 1. Deskripsi Proyek

Proyek ini melakukan pembersihan data (*data cleaning*) dan *Exploratory Data Analysis* (EDA) pada dataset katalog global tayangan **Netflix** (*Movies* & *TV Shows*) untuk memahami komposisi jenis tayangan, tren penambahan konten dari tahun ke tahun, negara produsen utama, serta distribusi *rating* usia penonton.

---

## 2. Tahapan Pengolahan Data

1. **Penanganan Nilai Kosong (*Missing Values*):**
   - Mengisi nilai kosong pada atribut `director`, `cast`, dan `country` dengan label `'Unknown'` agar data tetap dapat dianalisis tanpa membuang baris valid lainnya.
2. **Ekstraksi & Transformasi Fitur (*Feature Engineering*):**
   - Mengonversi kolom `date_added` menjadi tipe `datetime` dan mengekstrak tahun penambahan (`year_added`).
   - Memisahkan satuan durasi antara kategori **Movie** (dalam satuan menit, mis. `90 min`) dan **TV Show** (dalam satuan jumlah musim, mis. `2 Seasons`).
3. **Visualisasi & Analisis Pola:**
   - Proporsi jumlah **Movie** vs **TV Show** di dalam katalog.
   - Tren pertumbuhan rilis dan penambahan tayangan per tahun.
   - Distribusi 5 besar klasifikasi *rating* usia penonton (`TV-MA`, `TV-14`, `PG-13`, `R`, `TV-PG`).

---

## 3. Struktur File

```text
├── analisis_netflix.ipynb          # Notebook Jupyter tahapan Data Cleaning & EDA
├── data/
│   └── netflix_titles_sample.csv   # Sampel dataset katalog tayangan Netflix
├── requirements.txt                # Daftar pustaka Python
└── README.md                       # Dokumentasi proyek
```
