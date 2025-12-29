# Final-Project-Deep-Learning
**Deskripsi Final Project Deep Learning – Klasifikasi Gambar Pakaian**

Proyek ini bertujuan membangun sistem klasifikasi gambar pakaian menggunakan pendekatan deep learning, di mana model menerima input berupa gambar pakaian dan menghasilkan output label/kategori pakaian seperti dress, shirt, jacket, dan kategori lainnya. Dataset yang digunakan bersumber dari **DeepFashion – Attribute Prediction**, yang menyediakan ratusan ribu citra pakaian dengan anotasi kelas yang sangat detail, serta disimpan dan dikelola ulang melalui Google Drive untuk kebutuhan eksperimen.

Karena ukuran dataset awal sangat besar (±289.000 gambar), dilakukan proses filtering dan sampling sehingga dataset diperkecil menjadi sekitar *9.200 gambar* agar proses pelatihan lebih efisien dan sesuai dengan keterbatasan komputasi. Metode yang digunakan adalah **EfficientNet**, karena arsitektur ini mampu mengekstraksi fitur visual secara efektif dengan jumlah parameter yang relatif efisien.

Eksperimen dilakukan menggunakan **dua skema klasifikasi**. Model pertama adalah *Fine-Grained Model* yang mengklasifikasikan gambar ke dalam 64 kelas, sesuai detail kategori pakaian pada dataset. Dengan pelatihan awal selama 20 epoch, model ini mencapai akurasi sekitar 27%. Model kedua adalah *Coarse-Grained Model*, di mana kelas-kelas pakaian disederhanakan menjadi 4 kategori utama, yaitu blouse, jacket, blazer, dan coat. Dengan arsitektur dan konfigurasi pelatihan yang sama, model ini berhasil mencapai akurasi sebesar 88%. Peningkatan signifikan ini menunjukkan bahwa penyederhanaan jumlah kelas membantu model membedakan karakteristik visual antar kategori dengan lebih jelas.

Secara keseluruhan, proyek ini menunjukkan perbandingan performa fine-grained vs coarse-grained classification pada domain fashion, serta menegaskan bahwa kompleksitas jumlah kelas sangat berpengaruh terhadap kinerja model deep learning, khususnya pada dataset dengan perbedaan visual yang halus antar kelas.
