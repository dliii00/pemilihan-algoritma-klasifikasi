# Pemilihan Algoritma Klasifikasi

## 1. Pengertian

Pemilihan algoritma klasifikasi merupakan salah satu tahapan penting dalam proses *Machine Learning*. Setiap algoritma memiliki karakteristik, kelebihan, dan kekurangan yang berbeda. Oleh karena itu, pemilihan algoritma harus disesuaikan dengan jenis data, ukuran dataset, kompleksitas masalah, kecepatan komputasi, serta kebutuhan interpretabilitas model.

Tidak terdapat satu algoritma yang selalu memberikan hasil terbaik untuk semua permasalahan klasifikasi. Algoritma yang tepat ditentukan berdasarkan karakteristik dataset dan hasil evaluasi model.

## 2. Faktor yang Memengaruhi Pemilihan Algoritma

### A. Jenis Data dan Kompleksitas Permasalahan

Jenis data menjadi salah satu faktor yang memengaruhi pemilihan algoritma klasifikasi. Data dapat berupa numerik, kategorikal, maupun teks. Setiap jenis data membutuhkan proses pengolahan yang sesuai sebelum digunakan dalam klasifikasi.

Contohnya:
- **K-Nearest Neighbor (KNN):** cocok untuk permasalahan yang dapat diselesaikan menggunakan pendekatan kemiripan atau jarak antar data.
- **Logistic Regression:** cocok untuk klasifikasi dengan hubungan yang relatif linear antara fitur dan target.
- **Support Vector Machine (SVM):** dapat menangani pola linear maupun non-linear dengan pemilihan kernel yang sesuai.
- **Random Forest:** mampu menangani hubungan data yang kompleks melalui gabungan beberapa pohon keputusan.

Pada algoritma KNN, normalisasi data perlu diperhatikan karena perbedaan skala antaratribut dapat memengaruhi perhitungan jarak.

### B. Ukuran Dataset

Ukuran dataset juga memengaruhi pemilihan algoritma karena setiap algoritma memiliki kebutuhan komputasi yang berbeda.

Beberapa algoritma yang dapat dipertimbangkan:
- **Dataset kecil hingga menengah:** Logistic Regression, Naïve Bayes, dan KNN dapat dijadikan pilihan awal karena relatif sederhana untuk diterapkan.
- **Dataset besar:** Random Forest dan SVM dapat dipertimbangkan berdasarkan kompleksitas data dan kemampuan perangkat yang digunakan.

Namun, ukuran dataset bukan satu-satunya penentu. KNN, misalnya, dapat membutuhkan waktu prediksi lebih lama ketika jumlah data pelatihan meningkat karena harus menghitung jarak terhadap data yang tersedia.

### C. Kecepatan Komputasi dan Skalabilitas

Kecepatan komputasi penting terutama pada aplikasi yang membutuhkan hasil prediksi secara cepat atau *real time*.

Beberapa algoritma yang dapat dipertimbangkan:
- **Naïve Bayes:** memiliki proses perhitungan yang relatif sederhana dan efisien.
- **Logistic Regression:** memiliki proses prediksi yang relatif cepat.
- **KNN:** dapat membutuhkan waktu prediksi lebih lama karena menghitung jarak terhadap data pelatihan.
- **Random Forest:** waktu pelatihan dan prediksinya dipengaruhi oleh jumlah pohon yang digunakan.

Pemilihan algoritma perlu mempertimbangkan waktu pelatihan dan waktu prediksi agar model dapat bekerja sesuai kebutuhan sistem.

### D. Interpretabilitas Model

Interpretabilitas merupakan kemampuan untuk memahami proses pengambilan keputusan suatu model. Faktor ini penting dalam bidang kesehatan, keuangan, pendidikan, dan bidang lain yang membutuhkan transparansi.

Algoritma yang relatif mudah dipahami:
- **Decision Tree:** menghasilkan struktur pohon dan aturan keputusan yang mudah dibaca.
- **Logistic Regression:** memungkinkan interpretasi hubungan fitur terhadap kemungkinan kelas melalui koefisien model.

Sementara itu, Random Forest dan SVM dengan kernel non-linear umumnya lebih sulit dijelaskan secara langsung karena proses pembentukan keputusannya lebih kompleks.

### E. Evaluasi Kinerja Algoritma

Setelah algoritma dipilih, perlu dilakukan pengujian untuk mengetahui kemampuan model dalam melakukan klasifikasi.

Beberapa metrik evaluasi yang dapat digunakan:
- **Accuracy:** mengukur proporsi prediksi yang benar dari seluruh data.
- **Precision:** mengukur ketepatan prediksi pada kelas positif.
- **Recall:** mengukur kemampuan model menemukan seluruh data positif.
- **F1-Score:** merupakan rata-rata harmonis antara precision dan recall.

Penggunaan beberapa metrik diperlukan terutama ketika dataset memiliki distribusi kelas yang tidak seimbang (*imbalanced data*).

## 3. Contoh Penelitian Pendukung

Beberapa penelitian menunjukkan bahwa tidak ada algoritma yang selalu unggul dalam semua permasalahan.

1. Dhuhita et al. (2022) membandingkan Naïve Bayes, KNN, dan SVM. Hasil penelitian menunjukkan SVM memperoleh akurasi 89,24%, Naïve Bayes 88,29%, dan KNN 85,14%.

2. Amal et al. (2022) membandingkan Random Forest, Logistic Regression, SVM, dan IndoBERT dalam klasifikasi sentimen. SVM memperoleh F1-Score tertinggi sebesar 0,81.

3. Astari et al. (2023) membandingkan KNN, SVM, Random Forest, dan C4.5. Random Forest memperoleh akurasi tertinggi sebesar 83%.

4. Sharfina dan Ramadhan (2023) menunjukkan bahwa penerapan SMOTE pada dataset Hepatitis C dapat meningkatkan performa klasifikasi Random Forest, khususnya pada nilai recall.

5. Anggara et al. (2022) menggunakan Decision Tree dan Regresi Logistik untuk memprediksi kinerja pegawai. Kedua algoritma tersebut dipertimbangkan berdasarkan karakteristik target dan kebutuhan interpretasi hasil.

## 4. Kesimpulan

Pemilihan algoritma klasifikasi harus mempertimbangkan jenis data, ukuran dataset, kompleksitas masalah, kecepatan komputasi, dan interpretabilitas model.

Logistic Regression dan Naïve Bayes dapat menjadi pilihan awal untuk permasalahan yang membutuhkan model relatif sederhana. KNN dapat digunakan untuk klasifikasi berbasis kemiripan data. Random Forest dan SVM dapat dipertimbangkan untuk menangani pola data yang lebih kompleks. Sementara itu, Decision Tree dan Logistic Regression dapat digunakan ketika hasil klasifikasi perlu dijelaskan dengan lebih mudah.

Dengan demikian, algoritma terbaik bukan ditentukan hanya berdasarkan ukuran dataset, melainkan berdasarkan kesesuaian algoritma terhadap karakteristik data dan kebutuhan permasalahan yang dihadapi.

## 5. Daftar Pustaka

1. Dhuhita, W. M. P., Darmawan, M. F. K. A., Triana, L., & Ankisqiantari, N. (2022). Comparison of Supervised Learning Algorithm for Classification of Thesis Titles Based on Lecturer Fields. *Jurnal Teknik Informatika dan Sistem Informasi (JuTISI), 8*(2), 427–437. https://doi.org/10.28932/jutisi.v8i2.4960

2. Amal, M. I., Rahmasita, E. S., Suryaputra, E., & Rakhmawati, N. A. (2022). Sentiment Classification Analysis On Phone Identity Card Data Leaks Issues On Twitter. *Jurnal Teknik Informatika dan Sistem Informasi (JuTISI), 8*(3), 645–660. https://doi.org/10.28932/jutisi.v8i3.5483

3. Astari, M. R., Nuruzzaman, M. T., & Sugiantoro, B. (2023). Comparison of K-Nearest Neighbor, Support Vector Machine, Random Forest, and C4.5 Algorithms on Indoor Positioning System. *International Journal on Informatics for Development, 12*(1), 302–313. https://doi.org/10.14421/ijid.2023.3991

4. Sharfina, N., & Ramadhan, N. G. (2023). Analisis SMOTE Pada Klasifikasi Hepatitis C Berbasis Random Forest dan Naïve Bayes. *JOINTECS (Journal of Information Technology and Computer Science), 8*(1), 33–40. https://doi.org/10.31328/jointecs.v8i1.4456

5. Anggara, E. D., Widjaja, A., & Suteja, B. R. (2022). Prediksi Kinerja Pegawai sebagai Rekomendasi Kenaikan Golongan dengan Metode Decision Tree dan Regresi Logistik. *Jurnal Teknik Informatika dan Sistem Informasi (JuTISI), 8*(1), 218–234. https://doi.org/10.28932/jutisi.v8i1.4479
