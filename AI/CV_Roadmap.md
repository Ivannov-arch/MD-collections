Untuk beralih ke spesifik **Computer Vision (CV)**, fokus utamanya berubah dari memproses urutan teks (sekuensial) menjadi memproses matriks piksel (spasial). Karakteristik datanya berbeda, tetapi beberapa fondasi rekayasa perangkat lunaknya tetap sama.

Berikut adalah roadmap spesifik untuk menjadi **Computer Vision AI Engineer**:

---

## 1. Fondasi Matematika & Manipulasi Gambar

Di CV, gambar adalah matriks angka (RGB atau Grayscale). Anda wajib bersahabat dengan manipulasi matriks.

* **Matematika:** Aljabar Linier (Sangat krusial untuk transformasi matriks, rotasi, translasi, dan operasi kernel), Kalkulus (untuk optimasi fungsi kerugian).
* **Digital Image Processing (DIP):** Konsep dasar sebelum ada Deep Learning. Anda harus tahu cara kerja *thresholding*, *blurring/smoothing* (Gaussian), deteksi tepi (Canny/Sobel), harris corner detection, dan transformasi warna (RGB ke HSV/Grayscale).
* **Library Wajib:** **OpenCV** (kit darurat utama setiap CV Engineer), `PIL/Pillow`, dan `NumPy` (untuk manipulasi array gambar).

---

## 2. Klasik Computer Vision (Feature Engineering)

Sebelum era Deep Learning mendominasi, CV mengandalkan ekstraksi fitur manual. Memahami ini penting karena teknik ini sangat cepat dan hemat komputasi untuk kasus sederhana.

* **Ekstraksi Fitur:** SIFT, SURF, ORB, dan HOG (Histogram of Oriented Gradients).
* **Algoritma Klasik:** Menggunakan fitur di atas dengan classifier tradisional seperti SVM atau Random Forest untuk klasifikasi objek sederhana.

---

## 3. Deep Learning & CNN (The Core)

Ini adalah menu utama. Sebagian besar tugas CV modern diselesaikan menggunakan jaringan saraf tiruan yang dirancang khusus untuk gambar.

* **Convolutional Neural Networks (CNN):** Pahami secara mendalam konsep *Convolutional Layer*, *Pooling Layer*, *Stride*, *Padding*, dan *Receptive Field*.
* **Arsitektur Klasik & Populer:** ResNet (standar industri untuk *backbone*), VGG, EfficientNet, dan MobileNet (untuk perangkat dengan komputasi rendah/edge).
* **Framework DL:** **PyTorch** (sangat dominan di industri CV) atau TensorFlow/Keras. Gunakan ekosistem **Torchvision**.

---

## 4. Tugas Utama Computer Vision (Core Tasks)

Anda harus menguasai minimal tiga kategori tugas utama ini:

* **Image Classification:** Menentukan kategori dari satu gambar penuh (misal: "Kucing" atau "Anjing").
* **Object Detection:** Menentukan *apa* objeknya dan *di mana* lokasinya menggunakan *bounding box*.
* **Wajib Dikuasai:** Keluarga **YOLO (You Only Look Once)**—saat ini YOLOv8 hingga variasi terbarunya adalah standar industri untuk deteksi *real-time*. Pahami juga konsep Faster R-CNN untuk akurasi tinggi.


* **Image Segmentation:** Memprediksi label untuk setiap piksel (Semantic vs Instance Segmentation).
* **Arsitektur:** U-Net (sangat populer di medis), Mask R-CNN, dan **SAM (Segment Anything Model)** dari Meta.


* **Tugas Tambahan (Opsional tapi Nilai Plus):** *Keypoint Detection* (estimasi pose tubuh), *Optical Character Recognition* (OCR), dan *Object Tracking* (DeepSORT/ByteTRACK).

---

## 5. Era Modern: Vision-Language & Generative Vision

Sama seperti NLP yang bergeser ke LLM, Computer Vision saat ini sedang berkonvergensi dengan teks.

* **Vision-Language Models (VLM):** Model yang menjembatani teks dan gambar. Contoh utamanya adalah **CLIP** dari OpenAI (dasar dari pencarian gambar berbasis teks).
* **Generative AI untuk Gambar:** Memahami dasar-dasar **Diffusion Models** (Stable Diffusion, Midjourney) dan bagaimana melakukan kontrol gambar menggunakan teknik seperti **ControlNet**.
* **Vision Transformers (ViT):** Mengadaptasi arsitektur Transformer (dari NLP) untuk memproses *patches* gambar. Semakin banyak digunakan untuk model skala besar saat ini.

---

## 6. Deployment & Edge AI (The "Engineer" Part)

Model CV sering kali harus berjalan di video *live stream* dengan kamera berkecepatan tinggi (misal: CCTV, kamera pabrik, atau self-driving car). Latensi dan efisiensi adalah segalanya.

* **Model Optimization:** Mempercepat inferensi gambar menggunakan **TensorRT** (NVIDIA), **ONNX Runtime**, atau **OpenVINO** (Intel).
* **Edge AI Deployment:** Mendeploy model ke perangkat keras kecil seperti Raspberry Pi, Jetson Nano, atau integrasi ke aplikasi mobile/web (menggunakan TensorFlow Lite atau ONNX Web).
* **Video Pipeline Management:** Mengelola aliran video (video streaming) menggunakan tools seperti **DeepStream SDK** atau `GStreamer` agar pemrosesan tidak *bottleneck* di I/O kamera.

---

### Rekomendasi Proyek Portofolio

Untuk CV, visualisasi portofolio Anda adalah kunci utama. Buat demo video dari proyek Anda:

1. **Level Pemula:** Sistem absensi otomatis berbasis *Face Recognition* menggunakan OpenCV dan model pre-trained (seperti FaceNet).
2. **Level Menengah:** Deteksi pelanggaran lalu lintas (misal: pengendara tanpa helm) menggunakan YOLO, lalu integrasikan dengan pelacakan objek (Object Tracking) untuk menghitung jumlah pelanggaran dari video CCTV.
3. **Level Mahir:** Bangun sistem inspeksi cacat produk otomatis di jalur pabrik (Defect Detection) menggunakan Unsupervised Anomaly Detection atau Segmentation, optimasikan modelnya dengan TensorRT agar bisa berjalan di FPS tinggi pada perangkat Edge.

Apakah minat Anda di Computer Vision ini lebih ke arah aplikasi praktis industri (seperti otomatisasi pabrik/CCTV) atau ke arah Generative AI (seperti manipulasi gambar/desain)?