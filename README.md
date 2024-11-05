
# Stack Overflow Scrapping

Scrapper ini digunakan untuk mengambil data dari halaman pertanyaan di Stack Overflow, termasuk judul pertanyaan, konten, jumlah vote, tag, dan jawaban. Data hasil scrapping akan disimpan dalam format CSV untuk analisis lebih lanjut.

## File dan Folder

- **HasilScrapping_Request.csv**  
  File ini berisi data hasil scrapping dari halaman pertanyaan Stack Overflow, mencakup informasi seperti judul, ringkasan pertanyaan, konten, jumlah vote, dan tag.

- **stackedoverflow_scrapping_request.ipynb**  
  Notebook ini menggunakan library `requests` dan `BeautifulSoup` untuk mengambil dan mengurai konten HTML dari halaman pertanyaan Stack Overflow. Cocok digunakan untuk scraping data yang kontennya tidak memerlukan interaksi dinamis.

- **stackedoverflow_scrapping_selenium.ipynb**  
  Notebook ini menggunakan Selenium untuk menangani konten dinamis pada halaman pertanyaan Stack Overflow yang mungkin tidak dapat diakses sepenuhnya dengan `requests` dan `BeautifulSoup`.

- **Folder**  
  Terdapat satu folder yang berisi file scraping untuk memproses data jika URL pertanyaan sudah di-crawl sebelumnya.

## Penggunaan

### 1. Clone Repositori
Clone repositori ini ke direktori lokal Anda:
```bash
https://github.com/hadijahumaira/StackOverflow_Scrapping.git
```

### 2. Penggunaan File

#### **stackedoverflow_scrapping_request.ipynb**:
  - Buka notebook ini untuk melakukan Scraping dengan `requests` dan `BeautifulSoup`.
  - Jalankan setiap sel di notebook untuk memulai proses scarping dengan  mengambil detail seperti judul pertanyaan, konten, jumlah vote, tag, dan jawaban.
  - Data yang discaping disimpan ke dalam file CSV bernama `HasilScrapping_Request.csv`.

#### **stackedoverflow_scrapping_selenium.ipynb**:
  - Gunakan notebook ini jika halaman Stack Overflow yang akan di-scrape mengandung konten dinamis.
  - Pastikan WebDriver yang sesuai (misalnya, ChromeDriver) sudah diinstal dan kompatibel dengan versi browser Anda.
  - Selenium akan mengotomatisasi browser untuk memuat setiap halaman pertanyaan, berinteraksi jika diperlukan, dan mengurai konten halaman secara dinamis.
  - Data yang diekstraksi disimpan dalam file CSV bernama `HasilScrapping_Selenium.csv`.

## Prasyarat

Pastikan telah menginstal:
- `Python 3.x`
- Library yang diperlukan, yang dapat diinstal dengan menjalankan perintah berikut:
  ```bash
  pip install -r requirements.txt
  ```
  - **WebDriver** untuk Selenium (misalnya, ChromeDriver atau GeckoDriver). Pastikan versi WebDriver sesuai dengan versi browser yang Anda gunakan.
