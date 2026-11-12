# Calistung Ceria — Modul 1 TK

Permainan literasi, berhitung, pola & logika, dan telusur huruf untuk anak TK.
Produk fondasi **Toko Aplikasi Edukasi AwwanMahda** (pilot jenjang TK) dan template baku
untuk modul-modul berikutnya.

- **Live (v1, arsip acuan):** https://latihan-calistung-awwan-pwa.vercel.app/
- **Versi ini:** v2.0 — bangun ulang bersih dari audit 12 November 2026.

## Isi (19 aktivitas, ronde 10 soal)

- **Literasi & Bahasa (7):** Huruf Awal, Cari Huruf, Baca Kata, Huruf Hilang,
  Baca 3 Kata, Cerita Pendek, Susun Suku Kata.
- **Berhitung (8):** Hitung Benda, Cocokkan Jumlah, Tambah Benda, Kurangi Benda,
  Tambah Angka, Kurangi Angka, Lebih Besar/Kecil, Urutan Angka.
- **Pola & Logika (3):** Pola Ceria, Cari yang Berbeda, Tebak Gambar.
- **Menulis Awal (1):** Telusur Huruf A–Z dengan jari (canvas) — motorik pramenulis.

## Perbaikan dari v1 (hasil audit)

- P0: kunci Susun Suku Kata dibetulkan (Sa+pi = Sapi); petunjuk Tebak Gambar
  tidak lagi membocorkan gambar jawaban.
- P1: aktivitas telusur huruf dibangun (klaim "menulis awal" kini berisi);
  audio/TTS (Web Speech, id-ID) di semua soal; penomoran "Soal X dari 10" + bilah progres.
- P2: merek netral "Calistung Ceria" + nama anak dapat diisi orang tua/guru
  (tersimpan lokal); kata baca memakai huruf campuran (bukan kapital semua);
  mekanik Huruf Awal vs Cari Huruf dibedakan (bunyi awal vs bentuk huruf).

## Prinsip desain (dari Peta Materi TK)

- Mengikuti CP Fase Fondasi (Keputusan Kepala BSKAP 046/H/KR/2025): belajar lewat
  bermain bermakna; aplikasi **menstimulasi kesiapan belajar**, bukan janji instan bisa membaca.
- Sesi pendek 5–10 menit (10 soal), titik berhenti alami, saran kegiatan di luar
  layar di akhir setiap permainan; tanpa iklan, tanpa autoplay tanpa henti.

## Teknis

- Satu berkas `index.html` (HTML/CSS/JS vanilla, tanpa dependensi/CDN) +
  `manifest.webmanifest` + `sw.js` (PWA, cache-first, bisa offline) + `icon.svg`.
- Deploy: impor repo ini ke Vercel (preset: Other/static, tanpa build command).

## Struktur penamaan produk (baku proyek)

`Jenjang + Kelas + Semester + Mata Pelajaran` — modul ini: **TK · Modul 1 · Literasi & Numerasi Fondasi**.
