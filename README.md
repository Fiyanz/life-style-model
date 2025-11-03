# Life-Style: Prediksi Kalori dan Rekomendasi Latihan

Proyek machine learning untuk prediksi kalori makanan dan rekomendasi latihan berdasarkan gaya hidup pengguna.

## 🎯 Tujuan Proyek

### Alasan Pembuatan
- **Kesehatan Digital**: Membantu pengguna mengelola asupan kalori dan aktivitas fisik secara lebih efektif
- **Personalisasi**: Memberikan rekomendasi yang disesuaikan dengan profil dan kebutuhan individu
- **Otomatisasi**: Mengurangi kompleksitas perhitungan manual kalori dan perencanaan latihan

### Fokus Utama
1. **Model Prediksi Kalori**: Memprediksi kandungan kalori makanan berdasarkan metadata makanan
2. **Sistem Rekomendasi Latihan**: Merekomendasikan jenis dan intensitas latihan yang sesuai
3. **Integrasi Data**: Menggabungkan data makanan dan aktivitas untuk analisis holistik

## 📊 Dataset

### Sumber Data
Dataset utama berasal dari Kaggle: [Life Style Data](https://www.kaggle.com/datasets/jockeroika/life-style-data)

### File Dataset
Proyek ini menggunakan dua dataset utama:
- [`Final_data.csv`](dataset/Final_data.csv): Dataset utama dengan informasi kalori dan aktivitas
- [`meal_metadata.csv`](dataset/meal_metadata.csv): Metadata makanan untuk training model

## 🚀 Setup Proyek

### Prasyarat
- Python 3.8+
- uv package manager

### Instalasi dengan UV

1. **Install uv** (jika belum terinstall):
```bash
curl -LsSf https://astral.sh/uv/install.sh | sh
```

2. **Clone repository**:
```bash
git clone <repository-url>
cd life-style
```

3. **Setup environment dan install dependencies**:
```bash
# Buat virtual environment
uv venv

# Aktifkan virtual environment
source .venv/bin/activate  # Linux/Mac
# atau
.venv\Scripts\activate     # Windows

# Install dependencies
uv pip install -r pyproject.toml
```

4. **Verifikasi instalasi**:
```bash
python main.py
```

## 📁 Struktur Proyek

```
life-style/
├── main.py                 # Entry point aplikasi
├── pyproject.toml          # Konfigurasi dependencies
├── dataset/                # Data untuk training dan testing
│   ├── Final_data.csv      # Dataset utama
│   └── meal_metadata.csv   # Metadata makanan
├── notebook/               # Jupyter notebooks untuk eksperimen
│   └── training_model.ipynb # Training dan evaluasi model
└── README.md              # Dokumentasi proyek
```

## 🤖 Fitur Utama

### 1. Prediksi Kalori
- Input: Informasi makanan (nama, porsi, kategori)
- Output: Estimasi kalori yang akurat
- Model: Trained menggunakan data dari [`meal_metadata.csv`](dataset/meal_metadata.csv)

### 2. Rekomendasi Latihan
- Input: Profil pengguna (usia, berat, tinggi, target)
- Output: Rekomendasi jenis latihan dan durasi
- Basis: Analisis data aktivitas dari [`Final_data.csv`](dataset/Final_data.csv)

## 💻 Penggunaan

### Menjalankan Aplikasi
```bash
python main.py
```

### Training Model
Buka dan jalankan notebook untuk training:
```bash
jupyter notebook notebook/training_model.ipynb
```

## 🔧 Development

### Menambah Dependencies
```bash
uv add package-name
```

### Menjalankan Tests
```bash
uv run pytest
```

### Code Formatting
```bash
uv run black .
uv run isort .
```

## 📈 Roadmap

- [ ] Implementasi web interface
- [ ] Integrasi dengan API nutrisi eksternal
- [ ] Mobile app development
- [ ] Real-time tracking fitur
- [ ] Social features untuk motivasi

## 🤝 Kontribusi

1. Fork repository
2. Buat feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit changes (`git commit -m 'Add some AmazingFeature'`)
4. Push ke branch (`git push origin feature/AmazingFeature`)
5. Buat Pull Request

## 📄 Lisensi

Distributed under the MIT License. See `LICENSE` for more information.


---
*Dibuat dengan ❤️ untuk hidup yang lebih sehat*