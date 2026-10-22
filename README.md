# UTS Graf RetailRocket

## Deskripsi Tugas

Tugas ini merupakan **Ujian Tengah Semester (UTS)** pada mata kuliah *Graf dan Analisis Data* (Semester 7).  
Mahasiswa diminta untuk melakukan analisis pada dataset **RetailRocket** yang berisi data transaksi e‑commerce.  
Dataset terdiri dari file CSV yang memuat informasi:
- `events.csv` – setiap aksi (view, add‑to‑cart, purchase) beserta timestamp, user ID, item ID, dsb.
- `category_tree.csv` – hierarki kategori produk.
- `item_properties.csv` – atribut item (price, category, dll).

## Notebook Utama

File notebook **`uts_gsd_.ipynb`** berisi langkah‑langkah berikut:
1. **Import data** menggunakan `pandas` dan eksplorasi awal.
2. **Pembersihan data** (menghapus duplikat, mengisi nilai yang hilang).
3. **Analisis graf** dengan `networkx` untuk membangun jaringan interaksi user‑item.
4. **Visualisasi** menggunakan `matplotlib`/`seaborn` serta `pyvis` untuk menampilkan graf interaktif.
5. **Insight** berupa metrik penting (degree centrality, connected components, conversion rate per path, dll).
6. **Kesimpulan** dan saran peningkatan strategi penjualan.

> **Catatan:** Notebook dirancang agar dapat dijalankan secara selangkah dengan magic `%%time` untuk memantau performa. Pastikan semua dependensi ter‑install (`pandas`, `networkx`, `pyvis`, `matplotlib`, `seaborn`).

## Cara Menjalankan Notebook
```bash
# 1. Buat environment (misal dengan venv atau conda)
python -m venv venv
source venv/Scripts/activate  # Windows PowerShell

# 2. Instal dependensi
pip install -r requirements.txt  # file requirements.txt tersedia di repo

# 3. Buka notebook
jupyter notebook uts_gsd_.ipynb
```

## Upload ke GitHub
Repositori ini sudah di‑push ke GitHub. Untuk memperbarui, lakukan:
```bash
git add .
git commit -m "Update README and notebook"
git push origin main
```

---
*Repository ini bersifat publik/privat sesuai kebijakan Anda.*
