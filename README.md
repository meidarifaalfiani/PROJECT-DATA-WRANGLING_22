# PROJECT-DATA-WRANGLING_22
Proyek ini menganalisis hubungan antara kemiskinan dan cakupan imunisasi dasar lengkap di Indonesia. Meski imunisasi penting untuk mencegah penyakit dan mendukung SDGs, disparitas sosial ekonomi dan akses layanan kesehatan masih menyebabkan ketimpangan antarprovinsi. Hasil analisis diharapkan membantu penyusunan kebijakan kesehatan yang lebih rata
Keterangan pada dataset hasil_cleaning_csv:
Not a Number (NaN)
NaN digunakan secara standar dalam ilmu data untuk menandai nilai yang hilang (missing value) atau data yang tidak tersedia dalam suatu kolom. NaN bukan angka, bukan nol, dan bukan pula error melainkan penanda resmi bahwa suatu observasi tidak memiliki nilai yang valid.
Jika sebuah provinsi memiliki NaN pada kolom seperti:
Garis Kemiskinan – September
Jumlah Penduduk Miskin – September
Persentase Penduduk Miskin – September
Maka ini berarti data kemiskinan bulan September tidak tersedia untuk provinsi tersebut (umumnya karena BPS belum merilis atau data tidak tercantum dalam file asli)

Keterangan kolom:
1. kode_provinsi 
: merupakan kode numerik yang ditetapkan oleh Badan Pusat Statistik (BPS) untuk mengidentifikasi masing-masing provinsi. Nilai ini bersifat administratif dan tidak memiliki makna statistik kuantitatif selain sebagai penanda wilayah.
2. nama_provinsi
: menunjukkan nama provinsi tempat data dikumpulkan. Variabel ini bersifat kategorikal dan digunakan untuk menghubungkan data imunisasi dengan data kemiskinan pada wilayah yang sama.
3. persentase_penduduk_miskin
: menyatakan persentase penduduk yang berada di bawah garis kemiskinan di masing-masing provinsi. Nilai ini dihitung oleh BPS berdasarkan proporsi penduduk dengan pengeluaran per kapita bulanan yang berada di bawah garis kemiskinan. Satuan yang digunakan adalah persen (%).
4. garis_kemiskinan_maret
: dua variabel ini mencerminkan nilai garis kemiskinan per kapita per bulan (dalam Rupiah) pada bulan Maret. Garis kemiskinan mencakup komponen pengeluaran makanan dan non-makanan yang dibutuhkan untuk memenuhi kebutuhan dasar. Individu dengan pengeluaran di bawah nilai ini dikategorikan sebagai miskin. Nilai dinyatakan dalam Rupiah (Rp), bukan persen.
5. garis_kemiskinan_september
: dalam proses pembersihan data, seluruh nilai yang ditandai dengan ‘…’ diganti menjadi NaN (Not a Number). NaN digunakan sebagai penanda standar untuk data yang hilang (missing values). Dengan mengganti nilai ‘…’ menjadi NaN, analisis statistik dapat dilakukan secara lebih akurat karena nilai tersebut tidak akan diperlakukan sebagai angka valid dan tidak akan mempengaruhi perhitungan rata-rata, korelasi, maupun pemodelan.
6. jumlah_penduduk_miskin_maret
: variabel ini menunjukkan estimasi jumlah penduduk miskin pada bulan maret periode tersebut. Variabel ini menunjukkan jumlah penduduk miskin dalam satuan ribu orang. Misalnya, nilai 806.75 menunjukkan bahwa terdapat sekitar 806.750 orang yang tergolong miskin pada periode tersebut. Satuan "ribu" digunakan untuk mempermudah penyajian angka.
7. jumlah_penduduk_miskin_september
: dalam proses pembersihan data, seluruh nilai yang ditandai dengan ‘…’ diganti menjadi NaN (Not a Number). NaN digunakan sebagai penanda standar untuk data yang hilang (missing values). Dengan mengganti nilai ‘…’ menjadi NaN, analisis statistik dapat dilakukan secara lebih akurat karena nilai tersebut tidak akan diperlakukan sebagai angka valid dan tidak akan mempengaruhi perhitungan rata-rata, korelasi, maupun pemodelan.
8. persentase_penduduk_miskin_september
: dalam proses pembersihan data, seluruh nilai yang ditandai dengan ‘…’ diganti menjadi NaN (Not a Number). NaN digunakan sebagai penanda standar untuk data yang hilang (missing values). Dengan mengganti nilai ‘…’ menjadi NaN, analisis statistik dapat dilakukan secara lebih akurat karena nilai tersebut tidak akan diperlakukan sebagai angka valid dan tidak akan mempengaruhi perhitungan rata-rata, korelasi, maupun pemodelan.
9. imunisasi_hb0
: Satuan: Persentase (%). Persentase bayi yang menerima imunisasi Hepatitis B dosis 0 (HB-0) dalam 24 jam pertama setelah lahir.
10. imunisasi_bcg
: Satuan: Persentase (%). Persentase bayi yang menerima imunisasi BCG (mencegah tuberkulosis).
11. imunisasi_dpt_hb_hib
: Satuan: Persentase (%). Persentase bayi yang menerima imunisasi kombinasi DPT-HB-Hib (difteri, pertusis, tetanus, hepatitis B, Haemophilus influenzae tipe B).
Biasanya masuk ke cakupan imunisasi dasar lengkap.
12. imunisasi_polio
: Satuan: Persentase (%). Persentase bayi yang menerima imunisasi polio (OPV/IPV).
13. imunisasi_rubella
: Satuan: Persentase (%). Persentase bayi yang menerima imunisasi campak / MR (Measles-Rubella).
14. N
: Beberapa dataset imunisasi menyediakan variabel "n" yang menunjukkan jumlah bayi sasaran yang menjadi dasar perhitungan persentase imunisasi. Variabel ini bersifat numerik dan merepresentasikan jumlah bayi (satuan: orang, bukan persen). Total bayi yang menjadi sampel dalam perhitungan persentase imunisasi pada tiap provinsi tersebut.

