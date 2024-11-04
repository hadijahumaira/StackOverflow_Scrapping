# Stack Overflow Scrapping

Scrapper ini digunakan untuk mengambil data dari halaman pertanyaan Stack Overflow, termasuk judul pertanyaan, konten, jumlah vote, tag, dan jawaban. Data hasil crawling akan disimpan dalam format CSV untuk analisis lebih lanjut.

## File dan Penggunaan

- **HasilScrapping_Request.csv**:  
  File ini berisi data hasil scraping dari halaman pertanyaan di Stack Overflow, seperti judul, ringkasan pertanyaan, konten, jumlah vote, dan tag.

- **stackedoverflow_scrapping_request.ipynb**:  
  Notebook ini menggunakan library `requests` dan `BeautifulSoup` untuk mengambil dan mengurai konten HTML dari halaman pertanyaan Stack Overflow.

  **Penggunaan**:
  - Muat URL dari file `HasilCrawl_Request.csv`.
  - Crawl setiap halaman untuk mengambil detail seperti judul pertanyaan, konten, jumlah vote, tag, dan jawaban.
  - Simpan data yang diekstraksi ke dalam file CSV bernama `HasilScrapping_Request.csv`.
 
- **stackedoverflow_scrapping_selenium.ipynb**:  
  Notebook ini menggunakan Selenium untuk menangani konten dinamis pada halaman pertanyaan Stack Overflow yang mungkin tidak dapat diakses melalui `requests` dan `BeautifulSoup`.

  **Penggunaan**:
  - Pastikan WebDriver yang sesuai (misalnya, ChromeDriver) sudah terinstal dan kompatibel dengan versi browser Anda.
  - Selenium mengotomatisasi browser untuk memuat setiap halaman pertanyaan, berinteraksi jika diperlukan, dan mengurai konten halaman.
  - Data yang diekstraksi disimpan dalam file CSV bernama `HasilScrapping_Selenium.csv`.

---



