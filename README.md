# UTS-GRAF-DAVAN-157
Data dibagi menjadi dua periode waktu, yaitu P1 sebagai data historis dan P2 sebagai data pengujian.
P1: 22 Mei–21 Juni 2015.
P2: 23–29 Juni 2015.

aktivitas melihat produk jauh lebih sering terjadi dibandingkan aktivitas menambahkan produk ke keranjang atau melakukan transaksi. Artinya, interaksi pengguna tidak selalu berakhir pada pembelian. 
pada subset 50 node teraktif dan ambang cosine similarity 0,05, pola interaksi antar-visitor terlihat lebih terhubung daripada pola antar-item. 
Hasil KNN dan evaluasi rekomendasi
- Visitor terpilih: 145740.
- Jumlah item historis P1: 10.
- Jumlah item relevan pada P2: 3.
- Lima tetangga terdekat ditemukan dengan cosine similarity masing-masing sekitar 0,316228.
- Rekomendasi Top-3 dan Top-5 masih kosong.
- Nilai Hit@5 dan NDCG@5 tercatat 0.
  Nilai metrik tersebut belum bisa dianggap sebagai ukuran kinerja rekomendasi yang valid, karena model belum menghasilkan item rekomendasi untuk dievaluasi. Selain itu, hasil komposisi graf di Neo4j menunjukkan 0 interaksi untuk periode P2, sementara data P2 di Pandas berisi 141.378 baris. Perbedaan ini juga perlu diperiksa sebelum menarik kesimpulan akhir.
  tugas uas ini menunjukkan penerapan analisis graf untuk mempelajari interaksi pengguna dan produk pada data e-commerce. Analisis awal menemukan dominasi aktivitas melihat produk, matriks User–Item yang sangat sparse, serta perbedaan pola konektivitas pada proyeksi User dan Item.

Perhitungan cosine similarity dan pencarian tetangga KNN juga telah dilakukan sebagai dasar rekomendasi. Namun, penyimpanan relasi similarity di Neo4j dan pembentukan rekomendasi akhir masih memerlukan perbaikan. Oleh sebab itu, hasil evaluasi rekomendasi belum dapat dijadikan kesimpulan akhir mengenai performa model.
