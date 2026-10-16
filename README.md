# Netflix Data Cleaning

Project belajar data cleaning bertahap menggunakan dataset Netflix Movies and TV Shows dari Kaggle. Fokus: inspeksi awal, analisis missing values, cleaning per kolom, validasi, dan export hasil — tanpa mengubah dataset asli.

## Dataset

- Sumber: Kaggle — Netflix Movies and TV Shows
- File asli: `netflix_titles.csv` (root) dan salinannya di `data/netflix_titles.csv`
- Jangan mengubah file asli. Hasil cleaning disimpan ke `data/netflix_cleaned.csv` (dibuat nanti setelah cleaning selesai).

## Struktur Project

```
.
├── data/
│   └── netflix_titles.csv
├── notebooks/
│   └── netflix_data_cleaning.ipynb
├── requirements.txt
├── .gitignore
├── README.md
└── .venv/  # dibuat lokal, tidak di-commit
```

## Setup

```zsh
cd netflix-cleaning
python3 -m venv .venv
source .venv/bin/activate
pip install --upgrade pip
pip install -r requirements.txt
python -m ipykernel install --user --name=netflix-cleaning --display-name="Python (netflix-cleaning)"
```

Dependensi (`requirements.txt`): `pandas`, `jupyter`, `ipykernel`.

## Penggunaan di VS Code

1. Buka folder `netflix-cleaning` di VS Code.
2. `Cmd+Shift+P` > `Python: Select Interpreter` > pilih `./.venv/bin/python`.
3. Buka `notebooks/netflix_data_cleaning.ipynb` > `Select Kernel` > pilih `.venv` / `Python (netflix-cleaning)`.
4. Jalankan cell dari atas ke bawah.

Alternatif via terminal:

```zsh
source .venv/bin/activate
jupyter notebook notebooks/netflix_data_cleaning.ipynb
```

## Isi Notebook

1. Import Libraries
2. Load Dataset (`../data/netflix_titles.csv`)
3. Initial Data Inspection
4. Missing Value Analysis
5. Data Cleaning (per kolom)
6. Data Validation
7. Export Cleaned Dataset (`../data/netflix_cleaned.csv`)

Notebook saat ini masih kerangka kosong untuk diisi bertahap.

## Status

- [x] Setup environment dan kerangka notebook
- [ ] Inspeksi awal
- [ ] Analisis missing values
- [ ] Cleaning per kolom
- [ ] Validasi dan export
