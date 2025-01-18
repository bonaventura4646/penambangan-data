1.	Judul / Topik Project dan Identitas

Prediksi Hasil Inspeksi Kualitas Makanan Berdasarkan Data Fasilitas

Nama : Bonaventura G.A.N.
Nim : A11.2022.14437
Kelompok Kelas : A11.4517

2.	Ringkasan dan Permasalahan:

Dinas inspeksi makanan mengumpulkan data inspeksi reguler di berbagai fasilitas makanan. Tujuan utama adalah mengoptimalkan jadwal inspeksi agar fokus pada fasilitas dengan potensi pelanggaran tertinggi.

Masalah: Dapatkah hasil inspeksi sebelumnya dan faktor lain yang ada memprediksi apakah suatu fasilitas akan lulus atau gagal inspeksi?
Tujuan:

-	Membangun model prediktif untuk memprediksi hasil inspeksi (lulus/gagal) menggunakan fitur yang tersedia.
-	Mengoptimalkan efisiensi sumber daya dalam inspeksi makanan.


Model/Alur Penyelesaian:

1.	Pemahaman Data: Mengkaji dataset yang diberikan untuk memahami struktur dan fitur.

2.	Eksplorasi Data (EDA): Analisis fitur penting seperti pelanggaran, tingkat risiko, lokasi, dan alasan inspeksi.
3.	Pra-pemrosesan Data: Membersihkan data, menangani nilai hilang, dan encoding fitur kategorikal.
4.	Pembelajaran Mesin (Modeling): Membangun model untuk klasifikasi hasil inspeksi.

5.	Evaluasi Model: Mengukur performa model menggunakan metrik evaluasi

Bagan Alur:

Dataset -> Eksplorasi Data -> Pra-pemrosesan -> Pemodelan -> Evaluasi -> Prediksi 


3.	Penjelasan Dataset:

Dataset memiliki fitur seperti:

-	ID unik, lokasi, tipe fasilitas, dan tingkat risiko.

-	Hasil inspeksi sebagai target, dengan nilai seperti FAIL, PASS, dan lainnya.

EDA:

-	Distribusi kategori hasil inspeksi.

-	Analisis hubungan fitur seperti RiskLevel dan SectionViolations dengan hasil inspeksi.


Proses Features Dataset:

-	Pra-pemrosesan:

-	Menangani nilai kosong.

-	Encoding data kategorikal (e.g., OneHot/Label Encoding).

-	Feature Engineering:

-	Ekstraksi informasi waktu dari kolom tanggal.

-	Normalisasi fitur numerik.


4.	Proses Learning / Modeling

-	Model: Algoritma seperti Random Forest, Gradient Boosting, atau Neural Networks.

-	Pendekatan:

-	Split data menjadi train-test.

-	Melakukan hyperparameter tuning untuk model terbaik.

-	Cross-validation untuk generalisasi.
 

5.	Performa Model

Evaluasi dilakukan menggunakan metrik seperti:

-	Accuracy: Persentase prediksi yang benar.

-	F1-Score: Harmonis antara presisi dan recall.

-	Confusion Matrix: Untuk melihat distribusi prediksi.


6.	Diskusi Hasil dan Kesimpulan

Hasil: Identifikasi fitur penting yang memengaruhi prediksi hasil inspeksi (e.g., tingkat risiko tinggi berkorelasi dengan gagal inspeksi).
Kesimpulan:

-	Model memberikan wawasan berharga untuk membantu tim inspeksi memprioritaskan fasilitas.

-	Penggunaan data historis terbukti efektif untuk prediksi hasil inspeksi.
