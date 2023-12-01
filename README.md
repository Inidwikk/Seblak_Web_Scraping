_Repositori ini dibuat guna menambah portopolio dengan melakukan Web Scraping pada salah satu applikasi jual beli._

---

## Instructions and Cases

#### Case
Kamu ingin menambah pendapatanmu dengan berjualan. Namun, kamu tidak punya cukup modal untuk produksi barang dan hanya cukup untuk promosi, sehingga kamu memutuskan untuk menjalanan skema dropship di platform Tokopedia.

Kamu masih bingung akan berjualan apa dan teringat bahwa saat ini sedang viral seblak. Namun, kamu tidak yakin apakah benar bahwa masyarakat memiliki animo yang besar terhadap seblak.

Karena kamu lulusan bootcamp Data Science Hacktiv8, dengan kemampuan dan pengetahuan kamu, kamu ingin menganalisis bagaimana penjualan produk seblak di Tokopedia. Apakah orang suka, apakah banyak yang beli, dsb.

Tantangannya, kamu tidak punya data sama sekali selain yang terpampang pada website e-commerce Tokopedia. Oleh karena itu, perjalanan kamu dimulai dari pengambilan data menggunakan Web Scraping!

#### A. Web Scraping
1. Pengambilan data dari halaman pencarian kata kunci produk "seblak" pada platform Tokopedia.
  https://www.tokopedia.com/search?navsource=&page=1&q=seblak&srp_component_id=02.01.00.00&srp_page_id=&srp_page_title=&st=

2. Data yang diambil adalah `Nama Produk`, `Harga Produk`, `Penjual`, `Kota Toko`, `Banyaknya Terjual`, dan `Rating Produk`.

3. Mangambil informasi produk dari 10 halaman pencarian.

4. setelah berhasil scraping, Data akan disimpan ke pandas data frame dan kemudian diolah.

#### B. Data Preparation

1. Lakukan eksplorasi data sederhana:
2. Lakukan data cleaning:
  Pada data cleaning akan dilakukan handling missing value bila ada, mengubah bentuk data menjadi konsisten dan menyesuaikan tipe data, etc. 

#### C. Analysis
  Dalam melakukan analisa data ada 4 poin yang ingin ssaya ketahui:
1. Saya ingin menghitung rata-rata, median, standar deviasi, skewness, dan kurtosis dari harga produk, banyaknya produk terjual, dan rating dari produk tersebut.

2. Berapa potensi minimum dan maksimum pendapatan jika saya menjual produk seblak? Disini saya menggunakan confidence interval dengan level 95% untuk mendapatkan lower value dan upper value dari distribusi populasi pendapatan. (Saya menganggap data normal dan informasi produk terjual merupakan penjualan produk per bulan)

3. Saya ingin mengetahui apakah harga barang di Jabodetabek dan di luar Jabodetabek berbeda? mengingat biaya bahan baku di kedua lokasi berbeda. 

4. Apakah orang lebih cenderung suka dengan produk yang harganya murah? Disini saya akan melakukan uji korelasi dengan menganalisis nilai korelasi dan p-value

#### E. Conclusion
  Kesimpulan  berisis hasil analisis 4 poin diatas.