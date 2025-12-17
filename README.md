# Multimedia Studio (Praktikum #8)

Aplikasi Android berbasis **Jetpack Compose** untuk pengelolaan multimedia yang mencakup fitur Perekam Audio, Pemutar Audio & Video, serta Integrasi Kamera & Galeri. [cite_start]Proyek ini dikembangkan sebagai tugas Praktikum Modul #8 Mobile Programming [cite: 1-6].

## 📱 Fitur Utama

### 1. 🎙️ Audio Recorder & Player
* [cite_start]**Perekam Suara:** Merekam audio menggunakan `MediaRecorder` dan menyimpannya secara lokal dengan format `.mp4`[cite: 23].
* [cite_start]**Pemutar Audio:** Memutar file rekaman menggunakan **ExoPlayer** dengan kontrol *Play*, *Pause*, dan *Seekbar* interaktif[cite: 24].
* [cite_start]**Manajemen File:** Daftar rekaman yang bisa diubah namanya (*Rename*) atau dihapus (*Delete*)[cite: 32].

### 2. 🎬 Video Player Interaktif
* [cite_start]**Pemutar Video:** Memutar video dari penyimpanan lokal menggunakan library **Media3 ExoPlayer**[cite: 25].
* [cite_start]**Gesture Support:** Mendukung **Pinch-to-Zoom** dan **Pan** (geser) untuk memperbesar detail video saat diputar[cite: 28].
* [cite_start]**Fullscreen Mode:** Mendukung pemutaran layar penuh dengan orientasi landscape[cite: 27].

### 3. 📸 Camera & Gallery
* [cite_start]**Ambil & Pilih:** Mengambil foto baru via Kamera atau memilih media (foto/video) dari Galeri perangkat[cite: 15].
* [cite_start]**Preview Canggih:** Pratinjau gambar dengan dukungan gesture zoom dan geser tanpa berpindah layar [cite: 16-19].
* [cite_start]**Simpan ke Galeri:** Fitur untuk menyimpan foto hasil tangkapan aplikasi ke Galeri utama HP menggunakan *Scoped Storage* (MediaStore) [cite: 21-22].

## 🛠️ Teknologi & Library

* **Bahasa:** [Kotlin 2.0+](https://kotlinlang.org/)
* [cite_start]**UI Toolkit:** [Jetpack Compose](https://developer.android.com/jetpack/compose) (Material3) [cite: 68-70]
* **Media:**
    * [cite_start]`androidx.media3:media3-exoplayer` (Video & Audio) [cite: 82]
    * [cite_start]`android.media.MediaRecorder` (Audio Recording) [cite: 80]
* **Icons:** `androidx.compose.material:material-icons-extended`
* [cite_start]**Navigation:** Navigation Compose [cite: 72]

## 📂 Struktur Proyek

[cite_start]Struktur folder disusun berdasarkan fitur (*feature-based*) untuk memudahkan pengembangan [cite: 91-114]:

```text
id.antasari.p8_multimedia_nimanda
├── ui/
│   ├── gallery/    # Screen Kamera & Galeri
│   ├── home/       # Halaman Utama (Dashboard)
│   ├── player/     # Screen Pemutar Audio
│   ├── recorder/   # Screen Perekam Audio
│   ├── video/      # Screen Pemutar Video
│   ├── theme/      # Konfigurasi Tema & Warna
│   └── NavGraph.kt # Pengaturan Navigasi
├── util/           # Helper untuk manajemen file
└── MainActivity.kt
🚀 Cara Menjalankan
Clone repository ini ke komputer Anda.

Buka di Android Studio (Disarankan versi terbaru).

Tunggu proses Gradle Sync selesai.

Catatan: Pastikan koneksi internet stabil untuk mengunduh library ExoPlayer & Compose.

Hubungkan perangkat Android atau jalankan Emulator.

Berikan izin (Permission) untuk Microphone dan Camera saat aplikasi pertama kali dijalankan.

📝 Kredit
Mata Kuliah Mobile Programming S1 Teknologi Informasi - UIN Antasari Banjarmasin

Nama: Husni Majedi
NIM : 230104040123
Dosen Pengampu: Muhayat, M.IT
# Multimedia Studio (Praktikum #8)

Aplikasi Android berbasis **Jetpack Compose** untuk pengelolaan multimedia yang mencakup fitur Perekam Audio, Pemutar Audio & Video, serta Integrasi Kamera & Galeri. [cite_start]Proyek ini dikembangkan sebagai tugas Praktikum Modul #8 Mobile Programming [cite: 1-6].

## 📱 Fitur Utama

### 1. 🎙️ Audio Recorder & Player
* [cite_start]**Perekam Suara:** Merekam audio menggunakan `MediaRecorder` dan menyimpannya secara lokal dengan format `.mp4`[cite: 23].
* [cite_start]**Pemutar Audio:** Memutar file rekaman menggunakan **ExoPlayer** dengan kontrol *Play*, *Pause*, dan *Seekbar* interaktif[cite: 24].
* [cite_start]**Manajemen File:** Daftar rekaman yang bisa diubah namanya (*Rename*) atau dihapus (*Delete*)[cite: 32].

### 2. 🎬 Video Player Interaktif
* [cite_start]**Pemutar Video:** Memutar video dari penyimpanan lokal menggunakan library **Media3 ExoPlayer**[cite: 25].
* [cite_start]**Gesture Support:** Mendukung **Pinch-to-Zoom** dan **Pan** (geser) untuk memperbesar detail video saat diputar[cite: 28].
* [cite_start]**Fullscreen Mode:** Mendukung pemutaran layar penuh dengan orientasi landscape[cite: 27].

### 3. 📸 Camera & Gallery
* [cite_start]**Ambil & Pilih:** Mengambil foto baru via Kamera atau memilih media (foto/video) dari Galeri perangkat[cite: 15].
* [cite_start]**Preview Canggih:** Pratinjau gambar dengan dukungan gesture zoom dan geser tanpa berpindah layar [cite: 16-19].
* [cite_start]**Simpan ke Galeri:** Fitur untuk menyimpan foto hasil tangkapan aplikasi ke Galeri utama HP menggunakan *Scoped Storage* (MediaStore) [cite: 21-22].

## 🛠️ Teknologi & Library

* **Bahasa:** [Kotlin 2.0+](https://kotlinlang.org/)
* [cite_start]**UI Toolkit:** [Jetpack Compose](https://developer.android.com/jetpack/compose) (Material3) [cite: 68-70]
* **Media:**
    * [cite_start]`androidx.media3:media3-exoplayer` (Video & Audio) [cite: 82]
    * [cite_start]`android.media.MediaRecorder` (Audio Recording) [cite: 80]
* **Icons:** `androidx.compose.material:material-icons-extended`
* [cite_start]**Navigation:** Navigation Compose [cite: 72]

## 📂 Struktur Proyek

[cite_start]Struktur folder disusun berdasarkan fitur (*feature-based*) untuk memudahkan pengembangan [cite: 91-114]:

```text
id.antasari.p8_multimedia_nimanda
├── ui/
│   ├── gallery/    # Screen Kamera & Galeri
│   ├── home/       # Halaman Utama (Dashboard)
│   ├── player/     # Screen Pemutar Audio
│   ├── recorder/   # Screen Perekam Audio
│   ├── video/      # Screen Pemutar Video
│   ├── theme/      # Konfigurasi Tema & Warna
│   └── NavGraph.kt # Pengaturan Navigasi
├── util/           # Helper untuk manajemen file
└── MainActivity.kt
🚀 Cara Menjalankan
Clone repository ini ke komputer Anda.

Buka di Android Studio (Disarankan versi terbaru).

Tunggu proses Gradle Sync selesai.

Catatan: Pastikan koneksi internet stabil untuk mengunduh library ExoPlayer & Compose.

Hubungkan perangkat Android atau jalankan Emulator.

Berikan izin (Permission) untuk Microphone dan Camera saat aplikasi pertama kali dijalankan.


Mata Kuliah Mobile Programming S1 Teknologi Informasi - UIN Antasari Banjarmasin

Nama: Husni Majedi
NIM: 230104040123
Dosen Pengampu: Muhayat, M.IT
