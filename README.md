# Estetika Gambar menggunakan NASNetLarge

Ini adalah script Python untuk mengevaluasi estetika gambar menggunakan model NASNetLarge. Skrip ini memproses beberapa gambar dan mengurutkannya berdasarkan nilai estetika dari yang terbesar hingga terkecil.

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

Gambar-gambar ditampilkan dalam subplot 2x2 dengan urutan sesuai dengan nilai estetika. Setiap gambar juga dilengkapi dengan teks yang menunjukkan urutan dan nilai estetika.Silakan mencoba skrip ini dengan gambar-gambar Anda sendiri untuk mengevaluasi estetika mereka menggunakan model NASNetLarge.
