# Estetika Gambar menggunakan NASNetLarge

Ini adalah script Python untuk mengevaluasi estetika gambar menggunakan model NASNetLarge. Skrip ini memproses beberapa gambar dan mengurutkannya berdasarkan nilai estetika dari yang terbesar hingga terkecil.

## Cara kerja NASNetLarge
NASNetLarge adalah salah satu model arsitektur jaringan saraf konvolusi (Convolutional Neural Network/CNN) yang dirancang khusus untuk tugas pengenalan gambar. Model ini dikembangkan oleh Google Brain dan menggunakan pendekatan desain neural arsitektur pencarian (Neural Architecture Search/NAS) untuk mencapai performa yang tinggi dalam tugas klasifikasi gambar.

Berikut adalah beberapa langkah utama dalam cara kerja NASNetLarge:

1. Neural Architecture Search (NAS): NASNetLarge menggunakan pendekatan NAS untuk mencari arsitektur jaringan saraf yang optimal. Proses ini melibatkan pencarian otomatis dari berbagai arsitektur kandidat, di mana arsitektur-arsitektur ini dihasilkan dan dievaluasi secara otomatis untuk menemukan yang terbaik.

2. Struktur blok sel: NASNetLarge menggunakan struktur blok sel yang berulang untuk membangun arsitektur jaringan saraf. Blok sel adalah unit dasar yang terdiri dari beberapa operasi pengolahan gambar yang saling terhubung. Setiap blok sel memiliki beberapa cabang yang memungkinkan jaringan untuk mempelajari pola-pola yang berbeda secara paralel.

3. Skip connections: NASNetLarge juga menggunakan koneksi melompat (skip connections) antara blok-blok sel. Koneksi melompat ini memungkinkan aliran informasi langsung dari lapisan yang lebih awal ke lapisan yang lebih dalam dalam jaringan, memungkinkan jaringan untuk mengakses representasi-fitur yang lebih kaya.

4. Preprocessing: Sebelum gambar dimasukkan ke dalam NASNetLarge, gambar-gambar tersebut diubah ukurannya agar sesuai dengan ukuran input yang diharapkan oleh model. Selanjutnya, gambar-gambar tersebut juga dipreproses menggunakan fungsi preprocess_input yang dapat mengubah nilai piksel menjadi skala yang sesuai dan menerapkan normalisasi yang diperlukan.

5. Training dan Inferensi: Setelah arsitektur jaringan NASNetLarge dibangun, model tersebut dapat dilatih menggunakan data latih yang berlabel. Data latih tersebut digunakan untuk menyesuaikan bobot-bobot (weights) model agar dapat melakukan klasifikasi dengan akurasi yang tinggi. Setelah dilatih, model dapat digunakan untuk melakukan inferensi pada gambar-gambar baru, di mana model akan memberikan prediksi kelas untuk setiap gambar.

NASNetLarge memiliki tingkat akurasi yang tinggi dalam tugas pengenalan gambar dan telah digunakan secara luas dalam berbagai aplikasi komputer visi. Namun, penting untuk diingat bahwa implementasi dan performa model dapat bervariasi tergantung pada kerangka kerja (framework) dan pengaturan yang digunakan.

## Persyaratan
- Python 3.x
- Library yang dibutuhkan:
  - PIL (Python Imaging Library)
  - numpy
  - tensorflow
  - matplotlib

Pastikan Anda telah menginstal library-library di atas sebelum menjalankan skrip ini.

## Penggunaan
1. Simpan gambar-gambar yang ingin dievaluasi dalam direktori yang sama dengan skrip ini.
2. Ubah nilai `file_gambar` menjadi daftar nama file gambar yang ingin dievaluasi.
3. Jalankan skrip dengan menjalankan file Python ini.

Skrip akan memproses gambar-gambar tersebut menggunakan model NASNetLarge yang telah dilatih sebelumnya. Setelah memproses gambar-gambar, skrip akan mengurutkannya berdasarkan nilai estetika dari yang terbesar hingga terkecil.

Hasilnya akan ditampilkan dalam bentuk subplot dengan susunan 2x2. Setiap gambar akan ditampilkan dengan urutan dan nilai estetika yang sesuai di bawahnya. Gambar dengan nilai estetika terbaik akan ditandai dengan teks berwarna hijau, sedangkan gambar dengan nilai estetika terburuk akan ditandai dengan teks berwarna merah.

## Contoh Hasil
Berikut adalah contoh hasil yang dapat Anda harapkan dari skrip ini:
![](hasil.png)
Gambar-gambar ditampilkan dalam subplot 2x2 dengan urutan sesuai dengan nilai estetika. Setiap gambar juga dilengkapi dengan teks yang menunjukkan urutan dan nilai estetika.

Silakan mencoba skrip ini dengan gambar-gambar Anda sendiri untuk mengevaluasi estetika mereka menggunakan model NASNetLarge.


