# Klipza — AI Video Clipper & Studio Editor
**sebelumnya dikenal sebagai Plan to Short · by Plan to Product**

> [!NOTE]
> **Pengumuman Rebranding (`Plan to Short` ➔ `Klipza`):**
> Mulai versi **`v1.2.0`**, **Plan to Short** resmi berganti nama dan identitas visual menjadi **Klipza** (tetap dikembangkan oleh tim yang sama, **Plan to Product**).
> - **Lisensi Key lama (`P2P1-...`) tetap 100% berlaku** — tidak perlu membeli ulang atau mengganti lisensi.
> - **Proyek & folder alat media Anda tetap aman** dan langsung terbaca setelah update.
> - Nama repositori ini (`plan-to-short`) sengaja dipertahankan agar tautan unduhan lama dan fitur **Auto-Updater** tetap berjalan lancar tanpa kendala.

Aplikasi desktop Windows untuk memotong video panjang menjadi klip pendek vertikal & lanskap (`9:16`, `1:1`, `4:5`, `16:9`) siap upload ke TikTok, Reels, dan YouTube Shorts secara cepat, offline, dan ditenagai kecerdasan buatan (AI).

---

## Unduh & Instalasi (`v1.3.0`)

1. Buka halaman **[Releases](https://github.com/plantoproduct/plan-to-short/releases)** dan unduh file **`Klipza_1.3.0_x64-setup.exe`**.
2. Jalankan file installer dan ikuti instruksi pemasangan di layar.
3. Buka aplikasi **Klipza**, lalu masukkan **Lisensi Key** Anda untuk aktivasi.
4. Masuk ke menu **Pengaturan ➔ Alat Media**, pilih folder penyimpanan alat media (misalnya di Drive `D:\`), lalu pasang komponen yang dibutuhkan (`FFmpeg`, `yt-dlp`, `Pembuat transkrip` versi **CUDA GPU** untuk laptop NVIDIA, dan model teks Whisper).

---

## Yang Baru di `v1.3.0`

- **Live Filter Video Frame Preview:**
  - Seluruh 16 kartu preset filter warna kini menampilkan cuplikan/thumbnail asli dari frame video Anda secara real-time dengan efek grading visual yang akurat.
- **Smart Sentence Boundary Snapping (Anti-Terpotong):**
  - Algoritma pemotong momen AI kini menyelaraskan awal dan akhir klip persis pada batas kalimat utuh (tanda baca & jeda bicara alami), memastikan konteks percakapan tidak menggantung atau terpotong tanpa memakan memori tambahan.
- **Kinetic Clean Subtitles:**
  - Tanda baca berlebih (titik, koma, titik dua, kutip) pada ujung kata subtitle dibersihkan otomatis, menghasilkan tipografi subtitle modern, dinamis, dan nyaman dibaca cepat di platform video pendek.
- **Hook Visual Card & Dynamic Auto-Zoom:**
  - Pilihan Custom Card Visual Hook dengan styling clean, AI Hook Generator terarah, serta efek punch-in Auto-Zoom (+10% scale) saat pembuka video berjalan.
- **Branded Installer & Executable:**
  - Executable dan NSIS Setup resmi tersemat logo brand Klipza beresolusi tinggi di taskbar, shortcut, dan Windows Explorer.

---

## Yang Baru di `v1.2.0` (Arsip)

- **Optimasi Penuh Laptop NVIDIA (RTX / GTX):**
  - Pipeline ekspor **FFmpeg NVDEC + YUV-native + NVENC HQ** (3×–7× lebih cepat, menghindari bottleneck RGB CPU).
  - **Whisper AI GPU CUDA (12.4 / 11.8)** dengan Flash Attention hemat VRAM + fallback CPU otomatis jika VRAM penuh (5×–15× lebih cepat).
  - **Batch Ekspor Paralel 2×** untuk mode *Eksport Seluruh* + seluruh proses berat berjalan secara *asynchronous* (anti-freeze).
  - Dukungan otomatis laptop hybrid **NVIDIA Optimus** (`NvOptimusEnablement`) & diagnostik real-time VRAM/Driver/CUDA lewat `nvidia-smi`.
- **Watermark & Branding Channel:** Pasang teks `@username` atau **Logo PNG transparan** di 5 posisi dengan kontrol opasitas & ukuran, tampil real-time di preview & ter-burn ke `.mp4`.
- **Rebrand Resmi Klipza:** Identitas visual & ikon baru *Klipza by Plan to Product*.

---

## Fitur Utama

- **5 Template Studio + Ruang Kerja Multi-Proyek:** Kelola banyak proyek sekaligus di Sidebar dengan subtitle yang terkunci per klip.
- **Impor Link & File Lokal:** Mendukung link YouTube, TikTok, Instagram Reels, Facebook, X/Twitter, serta file video lokal (`MP4`, `MKV`, `MOV`, `WebM`).
- **8 Mode Framing & 16 Color Grade:** Layout otomatis (`Speaker Follow`, `Podcast Split`, `Gaming PIP`, `Full No-Crop`) dengan pratinjau real-time.
- **Subtitle Karaoke & Hook Card Interaktif:** Posisi, font, warna, dan highlight kata-per-kata langsung ter-render ke video `.mp4`.
- **Akselerasi GPU & CPU Otomatis:** Mendeteksi perangkat keras otomatis (NVIDIA CUDA/NVENC, AMD AMF, atau CPU Software Encoder).
- **Pembaruan Otomatis (Auto-Updater):** Cek dan pasang pembaruan langsung dari menu **Pengaturan ➔ Versi & Pembaruan**.

---

## Kebutuhan Sistem

- **OS:** Windows 10 / Windows 11 (64-bit)
- **Runtime:** Microsoft Edge WebView2 *(sudah terpasang bawaan di Windows 10/11 modern)*
- **Rekomendasi GPU:** NVIDIA GeForce GTX/RTX untuk akselerasi penuh CUDA + NVDEC/NVENC *(tetap berjalan lancar di mode CPU)*

---

© 2026 Plan to Product. All rights reserved.
