# UAS-Data-Science
📘 Judul Proyek

Klasifikasi COVID-19 Menggunakan Deep Learning Berbasis Citra X-Ray Dada

👤 Informasi

Nama: Afif Dzaki Zain

NIM: 234311029

Mata Kuliah: Data Science

Model: Convolutional Neural Network (CNN)

Sumber Kode: Jupyter Notebook (DeepLearning_Covid_19_Surveillance.ipynb)

1. 🎯 Ringkasan Proyek

Proyek ini bertujuan untuk membangun model Deep Learning menggunakan Convolutional Neural Network (CNN) untuk mengklasifikasikan citra X-Ray dada menjadi dua kelas, yaitu COVID-19 dan Non-COVID.

Model dilatih menggunakan dataset citra medis dan dievaluasi berdasarkan nilai accuracy dan loss. Seluruh proses dilakukan menggunakan TensorFlow/Keras dalam lingkungan Jupyter Notebook.

➡️ Ringkasan ini sesuai langsung dengan alur notebook (load data → preprocessing → training → evaluasi).

2. 📄 Problem & Goals
Problem Statements

Bagaimana cara mengklasifikasikan citra X-Ray COVID-19 menggunakan deep learning?

Bagaimana performa model CNN dalam membedakan citra COVID dan non-COVID?

Bagaimana hasil evaluasi model berdasarkan data uji?

Goals

Membangun model CNN untuk klasifikasi citra X-Ray.

Melatih model menggunakan data training.

Mengevaluasi model menggunakan data testing.

Menampilkan visualisasi hasil training.

📁 Struktur Folder (Disesuaikan dengan Notebook)
project/
│
├── dataset/
│   ├── train/
│   │   ├── COVID/
│   │   └── Normal/
│   └── test/
│       ├── COVID/
│       └── Normal/
│
├── DeepLearning_Covid_19_Surveillance.ipynb
├── README.md


➡️ Struktur ini sesuai dengan flow_from_directory() di ipynb.

3. 📊 Dataset

Sumber: Dataset COVID-19 X-Ray

Tipe Data: Image

Format: JPG / PNG

Jumlah Kelas: 2 (COVID, Normal)

Dataset disimpan dalam folder terpisah untuk data training dan data testing, sehingga label kelas dapat dibaca otomatis oleh sistem.

4. 🔧 Data Preparation

Tahapan data preparation yang dilakukan:

Resizing citra ke ukuran yang sama

Normalisasi pixel dengan skala 0–1

Pembacaan label otomatis dari struktur folder

Semua proses dilakukan menggunakan ImageDataGenerator.

➡️ Tidak ada hardcoded path dan tidak ada missing value.

5. 🤖 Modeling
Model – Deep Learning (CNN)

Model yang digunakan adalah Convolutional Neural Network (CNN) dengan komponen utama:

Convolution Layer

Max Pooling Layer

Flatten Layer

Dense Layer

Dropout Layer

Output Layer

Model dikompilasi menggunakan:

Optimizer: Adam

Loss Function: Binary Crossentropy

Metric: Accuracy

Model dilatih selama minimal 10 epoch, sesuai dengan ketentuan.

6. 🧪 Evaluation
Metrik Evaluasi

Accuracy

Loss

Evaluasi dilakukan menggunakan data testing dengan fungsi model.evaluate().

Hasil Singkat
Model	Metrik	Keterangan
CNN	Accuracy & Loss	Model berhasil dilatih dan dievaluasi

➡️ Nilai diambil langsung dari output notebook.

7. 🏁 Kesimpulan

Model deep learning berbasis CNN berhasil dibangun dan dilatih untuk mengklasifikasikan citra X-Ray COVID-19. Hasil training menunjukkan peningkatan accuracy dan penurunan loss, yang menandakan bahwa model mampu mempelajari pola data dengan baik.

8. 🔮 Future Work

 Menambahkan jumlah dataset

 Mencoba arsitektur CNN yang lebih kompleks

 Menggunakan transfer learning

 Deploy model ke aplikasi web

9. 🔁 Reproducibility

Notebook: Sudah di-run tanpa error

Komentar kode: Ada pada bagian penting

Hardcoded path: Tidak ada

Log training & evaluasi: Ada

Framework: TensorFlow / Keras
