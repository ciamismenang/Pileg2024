# Dashboard Target RW — PKS Ciamis

Halaman tambahan untuk repositori dashboard yang sudah ada (`index.html`, `data.js`, `geo.js`).

## File
- `target.html` — halaman dashboard target RW
- `target-data.js` — data dari Target_RW_PKS_Ciamis versi 2.1 (4 November 2026)
- memakai `geo.js` yang sudah ada di repositori (tidak perlu diunggah ulang)

## Cara memasang
1. Buka repositori dashboard di github.com → Add file → Upload files.
2. Unggah `target.html` dan `target-data.js` → Commit.
3. Setelah 1–2 menit halaman tersedia di `https://<username>.github.io/<nama-repo>/target.html`.
4. (Opsional) Tambahkan tautan di `index.html`, misalnya di dalam `<header>`:
   `<a href="target.html">Target RW →</a>`

## Isi
- Tingkat: Kabupaten → Dapil → Kecamatan → Desa → RW. Link bisa dibagikan per tingkat (contoh `target.html#/2/0/3`).
- Peta: tambahan target per desa (batas RW tidak tersedia).
- Tabel per wilayah atau daftar RW, dengan filter prioritas (P1/P2/P3) dan strategi (Mobilisasi/Persuasi).

## Memperbarui data
Bila file Target RW diperbarui, `target-data.js` dibuat ulang dari file Excel versi baru. Nomor versi dan tanggal tampil di bagian atas halaman.

## Catatan
GitHub Pages akun gratis membutuhkan repositori publik: siapa pun yang punya link bisa membuka halaman ini, termasuk prioritas dan target RW.
Data hanya angka agregat per wilayah; tidak memuat nama pemilih.
