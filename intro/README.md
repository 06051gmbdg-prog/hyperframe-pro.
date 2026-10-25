# Intro 5 Detik (HyperFrames)

Contoh intro video 5 detik, ukuran 1920x1080 (16:9), dibuat dengan [HyperFrames](https://github.com/heygen-com/hyperframes).

Isi animasi: latar gradien ungu-biru, cahaya yang membesar, garis yang memanjang, lalu judul dan subjudul yang muncul bergantian dan memudar di akhir.

## Kebutuhan

- Node.js 22 atau lebih baru
- FFmpeg

## Cara menjalankan

1. Buat proyek baru:

   ```bash
   npx hyperframes init intro-video
   cd intro-video
   ```

2. Ganti `index.html` di proyek itu dengan file `index.html` dari folder ini.

3. Lihat hasilnya di browser:

   ```bash
   npx hyperframes preview
   ```

4. Render ke MP4:

   ```bash
   npx hyperframes render
   ```

Membuka `index.html` langsung di browser tidak akan memutar animasi, karena timeline-nya dikendalikan oleh HyperFrames.

## Mengubah isi

- Teks: ubah `NAMA KANAL` dan `SELAMAT DATANG` di `index.html`.
- Warna: ubah nilai `linear-gradient` pada `#stage`.
- Durasi: ubah `data-duration` pada tiap elemen dan posisi waktu di bagian `<script>`.
- Ukuran: ubah `data-width` dan `data-height` pada `#stage`, serta `width` dan `height` pada CSS `#stage` (misalnya 1080x1920 untuk format vertikal).

## Catatan

Kode ini belum diuji render. Strukturnya mengikuti contoh di README resmi HyperFrames.
