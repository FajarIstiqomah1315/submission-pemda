## Nama: [Fajar Istiqomah]
## Email: [cdcc290d6x2058@student.devacademy.id]
## ID Peserta Coding Camp	[CDCC290D6X2058]
## Link Repository: https://github.com/FajarIstiqomah1315/submission-pemda/tree/master 

# 🛍️ ETL Pipeline - Fashion Studio Scraping Project

Project ini adalah implementasi ETL (Extract, Transform, Load) untuk mengambil data produk fashion dari website, membersihkan data, lalu menyimpannya ke dalam file CSV.

---

## 📌 Alur ETL Pipeline

### 1. Extract
Proses pengambilan data dari website:

- Sumber data: https://fashion-studio.dicoding.dev
- Menggunakan library `requests` dan `BeautifulSoup`
- Melakukan scraping dari beberapa halaman produk
- Data yang diambil:
  - Title
  - Price
  - Rating
  - Colors
  - Size
  - Gender

Output dari tahap ini berupa list data mentah.

---

### 2. Transform
Proses pembersihan dan transformasi data:

- Menghapus data yang kosong atau tidak valid
- Menstandarkan format data
- Mengubah data menjadi struktur yang siap dianalisis
- Menggunakan `pandas DataFrame`

Output berupa data yang sudah bersih.

---

### 3. Load
Proses penyimpanan data:

- Data hasil transform disimpan ke file CSV
- Nama file output: `products.csv`
- Menggunakan fungsi `to_csv()` dari pandas

---

## 🧪 Testing

Project ini menggunakan `pytest` untuk unit testing setiap modul.

### Menjalankan unit test:
```bash
python -m pytest tests
