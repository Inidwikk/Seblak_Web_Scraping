_Repositori ini dibuat guna menambah portopolio dengan melakukan Web Scraping pada salah satu applikasi jual beli._

---

## Instructions and Cases

#### Case
Kamu ingin menambah pendapatanmu dengan berjualan. Namun, kamu tidak punya cukup modal untuk produksi barang dan hanya cukup untuk promosi, sehingga kamu memutuskan untuk menjalanan skema dropship di platform Tokopedia.

Kamu masih bingung akan berjualan apa dan teringat bahwa saat ini sedang viral seblak. Namun, kamu tidak yakin apakah benar bahwa masyarakat memiliki animo yang besar terhadap seblak.

Karena kamu lulusan bootcamp Data Science Hacktiv8, dengan kemampuan dan pengetahuan kamu, kamu ingin menganalisis bagaimana penjualan produk seblak di Tokopedia. Apakah orang suka, apakah banyak yang beli, dsb.

Tantangannya, kamu tidak punya data sama sekali selain yang terpampang pada website e-commerce Tokopedia. Oleh karena itu, perjalanan kamu dimulai dari pengambilan data menggunakan Web Scraping!

#### A. Web Scraping
1. Lakukan pengambilan data dari halaman pencarian kata kunci produk "seblak". Kamu bisa langsung akses link ini:
  https://www.tokopedia.com/search?navsource=&page=1&q=seblak&srp_component_id=02.01.00.00&srp_page_id=&srp_page_title=&st=

2. Ambil data `Nama Produk`, `Harga Produk`, `Penjual`, `Kota Toko`, `Banyaknya Terjual`, dan `Rating Produk`.

3. Tokopedia memiliki skema promosi sehingga pada panel teratas merupakan info produk suatu merchant yang membayar iklan. Kita akan ambil produk di dalam box yang reguler dengan elemen `<div class="css-974ipl">`.

4. Ambil informasi produk minimal dari 10 halaman pencarian (perhatikan format url linknya dan eksplorasi terlebih dahulu halaman web nya).

5. Perlu diingat bahwa setiap orang dan setiap waktu akan menghasilkan hasil data yang berbeda, hal ini tidak masalah, yang paling penting jumlah data yang diperoleh minimal 50 data dari minimal 10 halaman yang diakses.

6. Simpan hasil scrape ke pandas data frame dan kemudian diolah. Kamu dibebaskan memberikan nama kolom yang memudahkan kamu.

#### B. Data Preparation

1. Lakukan eksplorasi data sederhana:
2. Lakukan data cleaning:
  Handling missing value bila ada, mengubah bentuk data menjadi konsisten dan menyesuaikan tipe data. 

#### C. Analysis
  Dalam melakukan analisa data untuk mencapai tujuan yang diinginkan, kamu perlu mengikuti soal/pertanyaan/instruksi berikut ini:
1. Hitung rata-rata, median, standar deviasi, skewness, dan kurtosis dari kolom harga, banyak produk terjual, dan rating. Dari hasil perhitungan, insight apa saja yang bisa kamu dapatkan khususnya terkait dengan produk seblak dan datanya (distribusi dan kecenderungan ada/tidaknya outlier)?

  **Note:** Jika menemukan adanya indikasi outlier dari perhitungan ini, tidak perlu dihandle karena sifatnya alami. Dibiarkan saja.

2. Kamu memikirkan berapa potensi minimum dan maksimum pendapatan jika kamu menjual produk seblak?(Gunakan confidence interval untuk mendapatkan lower value dan upper value dari distribusi populasi pendapatan).

  Anggap data terdistribusi normal dan informasi produk terjual merupakan penjualan produk per bulan. Ambil confidence level 95%.

3. Apakah harga barang di Jabodetabek dan di luar Jabodetabek berbeda? mengingat biaya bahan baku di kedua lokasi berbeda. (Gunakan uji hipotesis yang diawali dengan menuliskan hipotesis null dan alternatifnya serta tentukan jenis hipotesis yang digunakan).

4. Apakah orang lebih cenderung suka dengan produk yang harganya murah?

  Kamu dapat jawab pertanyaan ini dengan uji korelasi. Gunakan library scipy jangan pandas. Analisis nilai korelasi dan p-value nya. Gunakan teknik yang sesuai dengan kondisi data!

Kamu dilarang untuk copy-paste pertanyaan soal. Buat lah cerita yang runut dari persoalan dan jawaban nomor 1 sampai 4 sebagai ganti kalimat soal.

#### E. Conclusion
  Tuliskan di markdown kesimpulan dari hasil analisis dari nomor 1-4. Kesimpulan yang baik menjawab tujuan yang ingin dicapai. Kamu dibebaskan menuliskan dalam format paragraf atau poin.
