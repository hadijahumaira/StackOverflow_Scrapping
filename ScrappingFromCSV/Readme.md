# Stack Overflow Scrapping

Scrapper ini digunakan untuk mengambil data dari halaman pertanyaan Stack Overflow, termasuk judul pertanyaan, konten, jumlah vote, tag, dan jawaban. Data hasil scraping akan disimpan dalam format CSV untuk analisis lebih lanjut.

## File dan Penggunaan

- **HasilCrawl.csv**:  
  File ini berisi daftar URL dari pertanyaan-pertanyaan di Stack Overflow yang telah dicrawling sebelumnya dan akan di-scrape. Setiap URL harus berada dalam satu baris di bawah kolom `Link_question`.

- **stackedoverflow_scrapping_request.ipynb**:  
  Notebook ini menggunakan library `requests` dan `BeautifulSoup` untuk mengambil dan mengurai konten HTML dari halaman pertanyaan Stack Overflow.

  **Penggunaan**:
  - Muat URL dari file `HasilCrawl.csv`.
  - Crawl setiap halaman untuk mengambil detail seperti judul pertanyaan, konten, jumlah vote, tag, dan jawaban.
  - Simpan data yang diekstraksi ke dalam file CSV bernama `HasilScrappingWithCSV_Request.csv`.
 
- **stackedoverflow_scrapping_selenium.ipynb**:  
  Notebook ini menggunakan Selenium untuk menangani konten dinamis pada halaman pertanyaan Stack Overflow yang mungkin tidak dapat diakses melalui `requests` dan `BeautifulSoup`.

  **Penggunaan**:
  - Pastikan WebDriver yang sesuai (misalnya, ChromeDriver) sudah terinstal dan kompatibel dengan versi browser Anda.
  - Muat URL dari file `HasilCrawl.csv`.
  - Selenium mengotomatisasi browser untuk memuat setiap halaman pertanyaan, berinteraksi jika diperlukan, dan mengurai konten halaman.
  - Data yang diekstraksi disimpan dalam file CSV bernama `HasilScrappingWithCSV_Selenium.csv`.

---


